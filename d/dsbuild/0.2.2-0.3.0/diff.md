# Comparing `tmp/dsbuild-0.2.2-py3-none-any.whl.zip` & `tmp/dsbuild-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9837 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat        5 b- defN 21-Jul-19 13:00 dsbuild/.version
--rw-rw-rw-  2.0 fat      310 b- defN 21-Jul-08 07:58 dsbuild/__init__.py
--rw-rw-rw-  2.0 fat    22604 b- defN 21-Jul-19 12:57 dsbuild/__main__.py
--rw-rw-rw-  2.0 fat     4680 b- defN 21-Jul-08 07:58 dsbuild/version.py
--rw-rw-rw-  2.0 fat      265 b- defN 21-Jul-19 13:00 dsbuild-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-Jul-19 13:00 dsbuild-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       51 b- defN 21-Jul-19 13:00 dsbuild-0.2.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 21-Jul-19 13:00 dsbuild-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      688 b- defN 21-Jul-19 13:00 dsbuild-0.2.2.dist-info/RECORD
-9 files, 28703 bytes uncompressed, 8651 bytes compressed:  69.9%
+Zip file size: 10292 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 14:01 dsbuild/.version
+-rw-rw-rw-  2.0 fat      310 b- defN 23-Jun-26 12:24 dsbuild/__init__.py
+-rw-rw-rw-  2.0 fat    24670 b- defN 23-Jul-12 13:25 dsbuild/__main__.py
+-rw-rw-rw-  2.0 fat     4680 b- defN 23-Jun-26 12:24 dsbuild/version.py
+-rw-rw-rw-  2.0 fat      224 b- defN 23-Jul-12 14:01 dsbuild-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 14:01 dsbuild-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jul-12 14:01 dsbuild-0.3.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-12 14:01 dsbuild-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      688 b- defN 23-Jul-12 14:01 dsbuild-0.3.0.dist-info/RECORD
+9 files, 30727 bytes uncompressed, 9106 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: dsbuild/__main__.py
 Comment: 
 
 Filename: dsbuild/version.py
 Comment: 
 
-Filename: dsbuild-0.2.2.dist-info/METADATA
+Filename: dsbuild-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: dsbuild-0.2.2.dist-info/WHEEL
+Filename: dsbuild-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: dsbuild-0.2.2.dist-info/entry_points.txt
+Filename: dsbuild-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: dsbuild-0.2.2.dist-info/top_level.txt
+Filename: dsbuild-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dsbuild-0.2.2.dist-info/RECORD
+Filename: dsbuild-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dsbuild/.version

```diff
@@ -1 +1 @@
-0.2.2
+0.3.0
```

## dsbuild/__main__.py

```diff
@@ -11,15 +11,15 @@
 
 from argparse import ArgumentParser, RawTextHelpFormatter
 from collections import namedtuple
 from configparser import ConfigParser, NoSectionError
 from distutils.spawn import find_executable
 from pkg_resources import parse_version
 from setuptools import find_packages, find_namespace_packages
-
+from inspect import signature
 from .version import get_version
 from .__init__ import __version__
 
 # path to the directories
 _VENV_NAME = '.venv'
 _WHEELS_DIR_NAME = 'wheels'
 _BUILD_DIR_NAME = 'build'
@@ -180,58 +180,92 @@
     if changelog_path is None:
         changelog_path = os.path.join(get_project_root_dir(), 'Changelog.md')
 
     return get_version(changelog_path=changelog_path)
 
 
 ##################################################
-# Helpers to define the modes of this script.
+# Helpers to define the sub commands of this script.
 
-modes = dict()
 
-ModeFunction = namedtuple('ModeFunction', 'func description')
+def format_parser_description(subparsers):
+    """
+    Format the list of subparsers with their descriptions for the console.
 
+    Formatting is done by aligning the "<subparser name>: <subparser description>" lines
+    by a ":" symbol to achieve the following effect:
 
-def register(description):
-    def decorator_register(func):
-        global modes
-        function_prefix = 'mode_'
-        if not func.__name__.startswith(function_prefix):
-            raise ValueError(
-                f'Function name of a mode should start with a '
-                f"literal '{function_prefix}'."
-            )
-        modes[func.__name__[len(function_prefix) :]] = ModeFunction(func, description)
-        return func
+            short_name: description for the short name
+                  name: description for the name
+        very_long_name: description for the very long name
+
+    Args:
+        subparsers (List[ArgumentParser]): a name of the package to check.
+
+    Returns:
+        str: A formatted string (containing newline symbols) with the subparser names
+            and descriptions.
+    """
+    subparsers = {k: v.description for k, v in subparsers.choices.items()}
+    max_command_length = len(max(subparsers, key=len))
 
-    return decorator_register
+    formatted_descriptions = [
+        f'{k:>{max_command_length}}: {v}' for k, v in subparsers.items()
+    ]
+    return '\n'.join(formatted_descriptions)
 
 
-def get_valid_modes():
-    return list(modes.keys())
+def call_command(arguments):
+    """
+    Calls a function stored in `command_function` argument.
 
+    It requires the argument to contain a callable object under a `command_function`
+    argument as well as the arguments for all the function parameters.
 
-def format_mode_description():
-    max_len = len(max(get_valid_modes(), key=len))
+    This implementation is inspired by the trick described in the documentation of the
+    argparse subparsers functionality:
+    https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.add_subparsers
 
-    result = []
-    for k, v in modes.items():
-        result.append('{0:>{max_len}}: {1}'.format(k, v.description, max_len=max_len))
+    Arguments:
+        arguments (Namespace): an argparse namespace with the parsed arguments.
+    """
+    command_function = arguments.command_function
 
-    return '\n'.join(result)
+    command_parameters = signature(command_function).parameters.keys()
+    arguments = vars(arguments)
+
+    missing_arguments = set(command_parameters) - set(arguments)
+
+    if missing_arguments:
+        raise RuntimeError(
+            f'The following arguments are missing for a function call to '
+            '{command_function}: {list(missing_arguments)}'
+        )
+
+    kwargs = {k: arguments[k] for k in command_parameters}
+
+    return command_function(**kwargs)
 
 
 def read_dsbuild_config(config_path=None):
     """
     This function reads the config file that contains a dsbuild section.
-    If the file does not exist, the default config is returned.
+    If the file does not exist, the default config is returned, which
+    would look like this in the configuration file:
+
+    [dsbuild]
+    package_prefix =
+    test_dir = lib/tests
+    check_for_a_new_version = True
+    namespace_package_topdirs = ["lib"]
     """
     # default config
     dsbuild_conf = {
         'package_prefix': '',
+        'namespace_package_topdirs': '["lib"]',
         'test_dir': 'lib/tests',
         'check_for_a_new_version': True,
     }
 
     # default config path
     if config_path is None:
         config_path = os.path.join(get_project_root_dir(), 'setup.cfg')
@@ -248,14 +282,18 @@
         # if the [dsbuild] section does not exist, we just return defaults
         pass
 
     # Ensure boolean values
     for k in ['check_for_a_new_version']:
         dsbuild_conf[k] = dsbuild_conf[k] in [True, 'True', 'true', 'Yes', 'yes']
 
+    # load json serialized values
+    for k in ['namespace_package_topdirs']:
+        dsbuild_conf[k] = json.loads(dsbuild_conf[k])
+
     return dsbuild_conf
 
 
 def find_library(folder):
     """
     Find the python library in a folder and check if it is a normal library or part
     of a namespace package.
@@ -286,50 +324,52 @@
         package = package[0]
         is_namespace_pkg = True
     except IndexError:
         raise FileNotFoundError('No library could be found in:', folder)
     return os.path.join(folder, package), is_namespace_pkg
 
 
-def get_library_dirs():
+def get_library_dirs(toplevel_dirs_to_check):
     """
     Get the paths to the Python library-containing folders.
 
     A folder contains a library if it contains a `setup.py` file. There are two
     options:
     1. Simple library: A single `setup.py` file is present in the top-level.
     2. Namespace packages: Possibly multiple `setup.py` files can be found
                            underneath the `./lib` directory.
 
+   Args:
+        toplevel_dirs_to_check: required (List[str]):
+            List of folders (subfolders of project_root_dir) where Python library-containing folders will be searched.
+
     Returns:
         list of str:
             a list of folders that contain the python library
             (the folder containing the setup.py file)
     """
     project_root_dir = get_project_root_dir()
 
     # Option 1: Simple library, `setup.py` in top-level.
     if os.path.exists(os.path.join(project_root_dir, 'setup.py')):
         return [project_root_dir]
 
     # Option 2: Namespace packages.
-    setup_files = glob.glob(
-        os.path.join(project_root_dir, 'lib', '**', 'setup.py'), recursive=True
-    )
+    setup_files = []
+    for toplevel in toplevel_dirs_to_check:
+        setup_files += glob.glob(os.path.join(project_root_dir, toplevel, '**', 'setup.py'), recursive=True)
 
     return [os.path.dirname(f) for f in setup_files]
 
 
-@register(description='Print help.')
-def mode_help():
+def help():
     subprocess.check_call([sys.executable, __file__, '--help'])
 
 
-@register(description='Clean the project root directory to ensure a clean build.')
-def mode_clean():
+def clean():
     """
     Clean the root directory of the project to ensure a clean build.
     """
     dirs_to_clean = [_WHEELS_DIR_NAME, _BUILD_DIR_NAME, 'docs/build']
 
     project_root_dir = get_project_root_dir()
     for dirname in dirs_to_clean:
@@ -342,21 +382,21 @@
             raise OSError(
                 f"The folder '{path}' could not be deleted, "
                 'so we are not sure that all build files are fresh.'
             )
         print(f"Cleaned directory '{path}'.")
 
 
-@register(description='Build documentation.')
-def mode_docs():
+def docs():
     """
     Build the documentation.
     """
     lib_version = get_lib_version()
     project_root_dir = get_project_root_dir()
+    dsbuild_config = read_dsbuild_config()
 
     docs_dir = os.path.join(os.path.join(project_root_dir, 'docs'))
     if not os.path.exists(docs_dir):
         print(
             f"Directory '{docs_dir}' does not exist. "
             f'No documentation will be generated.'
         )
@@ -367,15 +407,15 @@
     source_dir = os.path.join(docs_dir, 'source')
 
     # python and sphinx-apidoc executable
     vpython = get_venv_python()
     sphinx_apidoc = get_venv_executable(executable='sphinx-apidoc.exe')
 
     # get all libraries
-    libs = get_library_dirs()
+    libs = get_library_dirs(dsbuild_config['namespace_package_topdirs'])
     if not libs:
         raise ValueError(f'No python libraries could be found in {project_root_dir}')
 
     # run sphinx-apidoc on all libraries
     for lib_dir in libs:
         lib_folder, is_namespace_pkg = find_library(lib_dir)
 
@@ -386,43 +426,41 @@
     library_name = os.path.basename(lib_folder)
 
     # run sphinx
     command = [vpython, '-m', 'sphinx', source_dir, html_dir]
     subprocess.check_call(command, cwd=project_root_dir)
 
     # Copy and version docs
-    dsbuild_config = read_dsbuild_config()
     package_name = dsbuild_config['package_prefix'] + library_name
     wheels_dir = os.path.abspath(os.path.join(project_root_dir, _WHEELS_DIR_NAME))
     wheels_lib_dir = os.path.join(wheels_dir, package_name)
     docs_dst = os.path.join(wheels_lib_dir, f'docs_{lib_version}')
     # TODO: The following will fail if `wheel_docs` already exists.
     shutil.copytree(src=html_dir, dst=docs_dst)
     print('Docs copied to:', docs_dst)
 
 
-@register(description='Publish the changelog file.')
-def mode_changelog():
+def changelog():
     """
     Publish the changelog file.
     """
     project_root_dir = get_project_root_dir()
     lib_version = get_lib_version()
+    dsbuild_config = read_dsbuild_config()
 
     # get all libraries
-    libs = get_library_dirs()
+    libs = get_library_dirs(dsbuild_config['namespace_package_topdirs'])
     if not libs:
         raise ValueError(f'No python libraries could be found in {project_root_dir}')
 
     for lib_dir in libs:
         lib_folder, is_namespace_pkg = find_library(lib_dir)
     library_name = os.path.basename(lib_folder)
 
     # define the target directory to save the changelog file in
-    dsbuild_config = read_dsbuild_config()
     # Take into account an optional "package prefix". This allows to create a package
     # `DS-imetric` with library `imetric`.
     package_name = dsbuild_config['package_prefix'] + library_name
     wheels_dir = os.path.abspath(os.path.join(project_root_dir, _WHEELS_DIR_NAME))
     wheels_lib_dir = os.path.join(wheels_dir, package_name)
 
     # Copy Changelog.md
@@ -438,26 +476,24 @@
 
         with open(changelog_dst, 'wt') as fid:
             fid.write(txt)
 
         print('Changelog copied to:', changelog_dst)
 
 
-@register(description='Build wheel.')
-def mode_wheel():
+def wheel():
     """
     Build a wheel of the library.
     """
     project_root_dir = get_project_root_dir()
     wheels_dir = os.path.abspath(os.path.join(project_root_dir, _WHEELS_DIR_NAME))
     all_build_dir = os.path.abspath(os.path.join(project_root_dir, _BUILD_DIR_NAME))
-
     dsbuild_config = read_dsbuild_config()
 
-    libraries = get_library_dirs()
+    libraries = get_library_dirs(dsbuild_config['namespace_package_topdirs'])
     if not libraries:
         raise ValueError(f'No python libraries could be found in {project_root_dir}')
 
     for library in libraries:
         lib_folder, is_namespace_pkg = find_library(library)
 
         if is_namespace_pkg:
@@ -483,38 +519,38 @@
             '-k',
         ]
         subprocess.check_call(command, cwd=library)
 
     print(f"Wheel(s) created in '{wheels_dir}'")
 
 
-@register(description='Run unittests + coverage.')
-def mode_test():
+def test():
     """
     Run unittests and coverage report. The tests are being picked up from a directory
     with name matching the pattern `*_test` or from `lib/tests`. Note that at most a
     single directory on disk should match. If not, this is considered a fatal error.
     """
     project_root_dir = get_project_root_dir()
+    dsbuild_config = read_dsbuild_config()
 
     # check if we can find libraries, otherwise raise exception
-    libs = get_library_dirs()
+    libs = get_library_dirs(dsbuild_config['namespace_package_topdirs'])
     if not libs:
         raise ValueError(f'No python libraries could be found in {project_root_dir}')
 
     # Get a list of (existing) folders that can contain tests.
     test_folders = []
     # 1. Legacy: dirs of the form `*_test`
     test_folders += [
         f
         for f in glob.glob(os.path.join(project_root_dir, '*_test'))
         if os.path.isdir(f)
     ]
     # 2. Custom (or new): By default `lib/tests`, but can be configured in `setup.cfg`.
-    dsbuild_config = read_dsbuild_config()
+
     test_dir = os.path.join(project_root_dir, dsbuild_config['test_dir'])
     test_folders += [f for f in [test_dir] if os.path.isdir(test_dir)]
 
     if len(test_folders) == 0:
         print(f'Could not find a folder with unittests. No tests will be run.')
         return
 
@@ -544,51 +580,29 @@
         f'--cov-report=html:{test_folder}_results/html',
     ]
     subprocess.check_call(command, cwd=project_root_dir)
 
     print('Ran all unittests.')
 
 
-@register(description='Print the library version.')
-def mode_version():
+def version(changelog):
     """
     Print library version.
-    """
-    parser = ArgumentParser(
-        prog='dsbuild version',
-        formatter_class=RawTextHelpFormatter,
-        description='Determine the version of a library.',
-    )
 
-    parser.add_argument(
-        '--changelog',
-        '-clog',
-        default=None,
-        help='Path to the Changelog.md file for version parsing.',
-    )
-
-    args = parser.parse_args(args=sys.argv[2:])
-
-    lib_version = get_lib_version(changelog_path=args.changelog)
+    Args:
+        changelog (str): An optional path to the changelog.
+    """
+    lib_version = get_lib_version(changelog_path=changelog)
     print(lib_version)
 
 
-@register(description='Generate a self-sufficient version.py at the project root.')
-def mode_generate_version_py():
+def generate_version_py():
     """
     Generate a self-sufficient version.py script.
     """
-    parser = ArgumentParser(
-        prog='dsbuild generate-version-py',
-        formatter_class=RawTextHelpFormatter,
-        description='Generate a self-sufficient version.py at the project root.',
-    )
-
-    args = parser.parse_args(args=sys.argv[2:])
-
     src = os.path.join(os.path.dirname(__file__), 'version.py')
     dst = os.path.join(get_project_root_dir(), 'version.py')
 
     with open(src, 'r') as fin, open(dst, 'w') as fout:
         header = (
             f'#########################################################################'
             f'###############\n'
@@ -608,60 +622,93 @@
 
         fout.write(header)
         fout.write(fin.read())
 
     print(f'Version.py file generated at {dst}')
 
 
-@register(description='clean + test + docs + wheel.')
-def mode_all():
+def all():
     """
     Convenience mode that does 'everything' from scratch (build, test, packaging).
     """
-    mode_clean()
-    mode_test()
-    mode_docs()
-    mode_wheel()
+    clean()
+    test()
+    docs()
+    wheel()
 
 
-@register(description='clean + docs + wheel.')
-def mode_package():
+def package():
     """
     Convenience mode that does a clean packaging.
     """
-    mode_clean()
-    mode_docs()
-    mode_wheel()
+    clean()
+    docs()
+    wheel()
 
 
 def main():
     parser = ArgumentParser(
-        prog='dsbuild',
-        formatter_class=RawTextHelpFormatter,
-        description=(
-            'This script helps to build and package python libraries.\n'
-            + format_mode_description()
-        ),
+        prog='dsbuild', formatter_class=RawTextHelpFormatter, description=(),
     )
     parser.add_argument(
         '--version', '-v', action='version', version=f'%(prog)s {__version__}'
     )
-    parser.add_argument(
-        'mode', default='all', const='all', nargs='?', choices=get_valid_modes()
+
+    subparsers = parser.add_subparsers()
+
+    sp = subparsers.add_parser(
+        'clean', description='Clean the project root directory to ensure a clean build.'
+    )
+    sp.set_defaults(command_function=clean)
+
+    sp = subparsers.add_parser('docs', description='Build documentation.')
+    sp.set_defaults(command_function=docs)
+
+    sp = subparsers.add_parser('changelog', description='Publish the changelog file.')
+    sp.set_defaults(command_function=changelog)
+
+    sp = subparsers.add_parser('wheel', description='Build wheel.')
+    sp.set_defaults(command_function=wheel)
+
+    sp = subparsers.add_parser('test', description='Run unittests + coverage.')
+    sp.set_defaults(command_function=test)
+
+    sp = subparsers.add_parser(
+        'version', description='Determine the version of a library.'
+    )
+    sp.add_argument(
+        '--changelog',
+        '-clog',
+        default=None,
+        help='Path to the Changelog.md file for version parsing.',
     )
+    sp.set_defaults(command_function=version)
 
-    # Only parse the mode argument here so that sub commands can parse the rest
-    args, _ = parser.parse_known_args(args=sys.argv[1:])
+    sp = subparsers.add_parser(
+        'generate-version-py',
+        description='Generate a self-sufficient version.py at the project root.',
+    )
+    sp.set_defaults(command_function=generate_version_py)
+
+    sp = subparsers.add_parser('all', description='clean + test + docs + wheel.')
+    sp.set_defaults(command_function=all)
+
+    sp = subparsers.add_parser('package', description='clean + docs + wheel.')
+    sp.set_defaults(command_function=package)
+
+    parser.description = (
+        f'This script helps to build and package python libraries.\n'
+        f'{format_parser_description(subparsers)}'
+    )
+
+    args = parser.parse_args()
 
     dsbuild_config = read_dsbuild_config()
 
     if dsbuild_config['check_for_a_new_version']:
         check_for_a_new_version('dsbuild', __version__)
 
-    try:
-        modes[args.mode].func()
-    except KeyError:
-        raise ValueError(f"Bad input mode '{args.mode}'.")
+    call_command(args)
 
 
 if __name__ == '__main__':
     main()
```

