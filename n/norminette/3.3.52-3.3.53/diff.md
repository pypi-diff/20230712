# Comparing `tmp/norminette-3.3.52.tar.gz` & `tmp/norminette-3.3.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norminette-3.3.52.tar", max compression
+gzip compressed data, was "norminette-3.3.53.tar", max compression
```

## Comparing `norminette-3.3.52.tar` & `norminette-3.3.53.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1057 2023-06-22 11:35:35.699121 norminette-3.3.52/LICENSE
--rw-r--r--   0        0        0     1384 2023-06-22 11:35:35.699121 norminette-3.3.52/README.md
--rw-r--r--   0        0        0      100 2023-06-22 11:35:35.699121 norminette-3.3.52/norminette/__init__.py
--rw-r--r--   0        0        0     4585 2023-06-22 11:35:35.699121 norminette-3.3.52/norminette/__main__.py
--rw-r--r--   0        0        0    22189 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/context.py
--rw-r--r--   0        0        0      191 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/exceptions.py
--rw-r--r--   0        0        0      173 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/dictionary.py
--rw-r--r--   0        0        0    18013 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/lexer.py
--rw-r--r--   0        0        0      626 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/lexer/tokens.py
--rw-r--r--   0        0        0     7072 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/norm_error.py
--rw-r--r--   0        0        0     4064 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/registry.py
--rw-r--r--   0        0        0     1041 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/__init__.py
--rw-r--r--   0        0        0     3080 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_assignation.py
--rw-r--r--   0        0        0     3234 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_assignation_indent.py
--rw-r--r--   0        0        0     1609 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_block_start.py
--rw-r--r--   0        0        0     1894 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_brace.py
--rw-r--r--   0        0        0     1159 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_comment.py
--rw-r--r--   0        0        0      664 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_comment_line_len.py
--rw-r--r--   0        0        0     2572 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_control_statement.py
--rw-r--r--   0        0        0      541 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_declaration.py
--rw-r--r--   0        0        0     2521 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_empty_line.py
--rw-r--r--   0        0        0      834 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_enum_var_decl.py
--rw-r--r--   0        0        0     2497 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_expression_statement.py
--rw-r--r--   0        0        0     4684 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_func_arguments_name.py
--rw-r--r--   0        0        0     2786 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_func_declaration.py
--rw-r--r--   0        0        0     1682 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_func_spacing.py
--rw-r--r--   0        0        0      496 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_functions_count.py
--rw-r--r--   0        0        0      885 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_general_spacing.py
--rw-r--r--   0        0        0     1182 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_global_naming.py
--rw-r--r--   0        0        0     2273 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_header.py
--rw-r--r--   0        0        0     1418 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_identifier_name.py
--rw-r--r--   0        0        0     1540 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_in_header.py
--rw-r--r--   0        0        0      562 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_label.py
--rw-r--r--   0        0        0     1104 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_line_count.py
--rw-r--r--   0        0        0     2045 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_line_indent.py
--rw-r--r--   0        0        0      558 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_line_len.py
--rw-r--r--   0        0        0     1100 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_many_instructions.py
--rw-r--r--   0        0        0     2938 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_nest_line_indent.py
--rw-r--r--   0        0        0     1030 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_newline_indent.py
--rw-r--r--   0        0        0    16112 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_operators_spacing.py
--rw-r--r--   0        0        0     5546 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_define.py
--rw-r--r--   0        0        0     2042 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_include.py
--rw-r--r--   0        0        0     1922 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_indent.py
--rw-r--r--   0        0        0     2145 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_preprocessor_protection.py
--rw-r--r--   0        0        0     3452 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_prototype_indent.py
--rw-r--r--   0        0        0     2394 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_spacing.py
--rw-r--r--   0        0        0     1218 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_struct_naming.py
--rw-r--r--   0        0        0      438 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_ternary.py
--rw-r--r--   0        0        0     6726 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_utype_declaration.py
--rw-r--r--   0        0        0     2996 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_variable_declaration.py
--rw-r--r--   0        0        0     5223 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/check_variable_indent.py
--rw-r--r--   0        0        0      705 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_ambiguous_declaration.py
--rw-r--r--   0        0        0     2935 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_assignation.py
--rw-r--r--   0        0        0     2302 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_block_end.py
--rw-r--r--   0        0        0     1897 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_block_start.py
--rw-r--r--   0        0        0     1211 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_cast.py
--rw-r--r--   0        0        0      464 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_comment.py
--rw-r--r--   0        0        0     3644 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_control_statement.py
--rw-r--r--   0        0        0      941 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_declaration.py
--rw-r--r--   0        0        0      687 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_empty_line.py
--rw-r--r--   0        0        0     3298 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_enum_var_decl.py
--rw-r--r--   0        0        0     4819 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_expression_statement.py
--rw-r--r--   0        0        0     8095 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_func_declaration.py
--rw-r--r--   0        0        0     7656 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_func_prototype.py
--rw-r--r--   0        0        0     3286 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_function_call.py
--rw-r--r--   0        0        0      652 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_label.py
--rw-r--r--   0        0        0     1180 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_preprocessor_statement.py
--rw-r--r--   0        0        0      730 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_ternary.py
--rw-r--r--   0        0        0     2798 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_user_defined_type.py
--rw-r--r--   0        0        0     7392 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/is_var_declaration.py
--rw-r--r--   0        0        0      821 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/rules/rule.py
--rwxr-xr-x   0        0        0      288 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/run_test.sh
--rw-r--r--   0        0        0     3382 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/scope.py
--rw-r--r--   0        0        0      949 2023-06-22 11:35:35.703121 norminette-3.3.52/norminette/tools/colors.py
--rw-r--r--   0        0        0      914 2023-06-22 11:35:35.743118 norminette-3.3.52/pyproject.toml
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 norminette-3.3.52/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-07-12 08:58:17.103168 norminette-3.3.53/LICENSE
+-rw-r--r--   0        0        0     1384 2023-07-12 08:58:17.103168 norminette-3.3.53/README.md
+-rw-r--r--   0        0        0      100 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/__init__.py
+-rw-r--r--   0        0        0     4609 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/__main__.py
+-rw-r--r--   0        0        0    22933 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/context.py
+-rw-r--r--   0        0        0      191 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/exceptions.py
+-rw-r--r--   0        0        0      173 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/lexer/__init__.py
+-rw-r--r--   0        0        0     2041 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/lexer/dictionary.py
+-rw-r--r--   0        0        0    16786 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/lexer/lexer.py
+-rw-r--r--   0        0        0      695 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/lexer/tokens.py
+-rw-r--r--   0        0        0     8342 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/norm_error.py
+-rw-r--r--   0        0        0     4064 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/registry.py
+-rw-r--r--   0        0        0      974 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/__init__.py
+-rw-r--r--   0        0        0     3080 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/check_assignation.py
+-rw-r--r--   0        0        0     3234 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/check_assignation_indent.py
+-rw-r--r--   0        0        0     1609 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/check_block_start.py
+-rw-r--r--   0        0        0     1894 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/check_brace.py
+-rw-r--r--   0        0        0     1159 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/check_comment.py
+-rw-r--r--   0        0        0      664 2023-07-12 08:58:17.103168 norminette-3.3.53/norminette/rules/check_comment_line_len.py
+-rw-r--r--   0        0        0     2572 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_control_statement.py
+-rw-r--r--   0        0        0      541 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_declaration.py
+-rw-r--r--   0        0        0     2443 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_empty_line.py
+-rw-r--r--   0        0        0      834 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_enum_var_decl.py
+-rw-r--r--   0        0        0     2497 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_expression_statement.py
+-rw-r--r--   0        0        0     4684 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_func_arguments_name.py
+-rw-r--r--   0        0        0     2824 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_func_declaration.py
+-rw-r--r--   0        0        0     1682 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_func_spacing.py
+-rw-r--r--   0        0        0      496 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_functions_count.py
+-rw-r--r--   0        0        0      885 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_general_spacing.py
+-rw-r--r--   0        0        0     1182 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_global_naming.py
+-rw-r--r--   0        0        0     2273 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_header.py
+-rw-r--r--   0        0        0     1418 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_identifier_name.py
+-rw-r--r--   0        0        0     1379 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_in_header.py
+-rw-r--r--   0        0        0      774 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_label.py
+-rw-r--r--   0        0        0     1104 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_line_count.py
+-rw-r--r--   0        0        0     2045 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_line_indent.py
+-rw-r--r--   0        0        0      558 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_line_len.py
+-rw-r--r--   0        0        0     1100 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_many_instructions.py
+-rw-r--r--   0        0        0     2938 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_nest_line_indent.py
+-rw-r--r--   0        0        0     1030 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_newline_indent.py
+-rw-r--r--   0        0        0    16112 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_operators_spacing.py
+-rw-r--r--   0        0        0     2006 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_preprocessor_define.py
+-rw-r--r--   0        0        0     2038 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_preprocessor_include.py
+-rw-r--r--   0        0        0     3331 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_preprocessor_indent.py
+-rw-r--r--   0        0        0     2627 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_preprocessor_protection.py
+-rw-r--r--   0        0        0     3452 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_prototype_indent.py
+-rw-r--r--   0        0        0     2423 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_spacing.py
+-rw-r--r--   0        0        0     1218 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_struct_naming.py
+-rw-r--r--   0        0        0      438 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_ternary.py
+-rw-r--r--   0        0        0     6726 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_utype_declaration.py
+-rw-r--r--   0        0        0     2996 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_variable_declaration.py
+-rw-r--r--   0        0        0     5223 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/check_variable_indent.py
+-rw-r--r--   0        0        0      705 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_ambiguous_declaration.py
+-rw-r--r--   0        0        0     2935 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_assignation.py
+-rw-r--r--   0        0        0     2302 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_block_end.py
+-rw-r--r--   0        0        0     2051 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_block_start.py
+-rw-r--r--   0        0        0     1211 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_cast.py
+-rw-r--r--   0        0        0      464 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_comment.py
+-rw-r--r--   0        0        0     3644 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_control_statement.py
+-rw-r--r--   0        0        0      941 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_declaration.py
+-rw-r--r--   0        0        0      687 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_empty_line.py
+-rw-r--r--   0        0        0     3298 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_enum_var_decl.py
+-rw-r--r--   0        0        0     4819 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_expression_statement.py
+-rw-r--r--   0        0        0     8036 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_func_declaration.py
+-rw-r--r--   0        0        0     7495 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_func_prototype.py
+-rw-r--r--   0        0        0     3286 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_function_call.py
+-rw-r--r--   0        0        0      840 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_label.py
+-rw-r--r--   0        0        0    12950 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_preprocessor_statement.py
+-rw-r--r--   0        0        0      744 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_ternary.py
+-rw-r--r--   0        0        0     2798 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_user_defined_type.py
+-rw-r--r--   0        0        0     7392 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/is_var_declaration.py
+-rw-r--r--   0        0        0      821 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/rules/rule.py
+-rwxr-xr-x   0        0        0      288 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/run_test.sh
+-rw-r--r--   0        0        0     3382 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/scope.py
+-rw-r--r--   0        0        0      949 2023-07-12 08:58:17.107168 norminette-3.3.53/norminette/tools/colors.py
+-rw-r--r--   0        0        0      914 2023-07-12 08:58:17.143169 norminette-3.3.53/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 norminette-3.3.53/PKG-INFO
```

### Comparing `norminette-3.3.52/LICENSE` & `norminette-3.3.53/LICENSE`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/README.md` & `norminette-3.3.53/README.md`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/__main__.py` & `norminette-3.3.53/norminette/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 elif os.path.isdir(arg):
                     if arg[-1] != "/":
                         arg = arg + "/"
                     targets.extend(glob.glob(arg + "**/*.[ch]", recursive=True))
                 elif os.path.isfile(arg):
                     targets.append(arg)
     event = []
-    for target in targets:
+    for target in filter(os.path.isfile, targets):
         if target[-2:] not in [".c", ".h"]:
             print(f"Error: {target} is not valid C or C header file")
         else:
             try:
                 event.append(Event())
                 if content is None:
                     with open(target) as f:
```

### Comparing `norminette-3.3.52/norminette/context.py` & `norminette-3.3.53/norminette/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from dataclasses import dataclass, field
+
 from norminette.exceptions import CParsingError
 from norminette.norm_error import NormError, NormWarning
 from norminette.scope import GlobalScope, ControlStructure
 from norminette.tools.colors import colors
 
 types = [
     "CHAR",
@@ -134,14 +136,47 @@
 sign_specifiers = ["SIGNED", "UNSIGNED"]
 
 whitespaces = ["SPACE", "TAB", "ESCAPED_NEWLINE", "NEWLINE"]
 
 arg_separator = ["COMMA", "CLOSING_PARENTHESIS"]
 
 
+@dataclass
+class Macro:
+    name: str
+    is_func: bool = field(default=False)
+
+    @classmethod
+    def from_token(self, token, **kwargs):
+        name = token.value or token.type
+        return Macro(name, **kwargs)
+
+
+class PreProcessors:
+    def __init__(self) -> None:
+        self.indent = 0
+
+        self.macros = []
+        self.includes = []
+
+        self.total_ifs = 0
+        self.total_elifs = 0
+        self.total_elses = 0
+        self.total_ifdefs = 0
+        self.total_ifndefs = 0
+
+        self.skip_define = False
+
+    def has_macro_defined(self, name):
+        for macro in self.macros:
+            if macro.name == name:
+                return True
+        return False
+
+
 class Context:
     def __init__(self, filename, tokens, debug=0, added_value=[]):
         # Header relative informations
         self.header_started = False
         self.header_parsed = False
         self.header = ""
         # File relative informations
@@ -160,36 +195,33 @@
         self.scope = GlobalScope()
         self.func_alignment = 0
         self.sub = None
         self.fname_pos = 0
         self.arg_pos = [0, 0]
 
         # Preprocessor handling
-        self.preproc_scope_indent = 0
-        self.skip_define_error = (
-            True if added_value is not None and "CheckDefine" in added_value else False
-        )
+        self.protected = False
+        self.preproc = PreProcessors()
+        self.preproc.skip_define = "CheckDefine" in (added_value or [])
 
     def peek_token(self, pos):
         return self.tokens[pos] if pos < len(self.tokens) else None
 
     def pop_tokens(self, stop):
         self.tokens = self.tokens[stop:]
 
     def check_token(self, pos, value):
         """Compares the token at 'pos' against a value or list of values"""
         tkn = self.peek_token(pos)
 
         if tkn is None:
             return None
 
-        if isinstance(value, list):
-            if tkn.type in value:
-                return True
-            return False
+        if isinstance(value, (tuple, list)):
+            return tkn.type in value
 
         return tkn.type == value
 
     def find_in_scope(self, value, nested=True):
         nests = 0
         for i in range(0, self.tkn_scope):
             tkn = self.peek_token(i)
@@ -271,18 +303,20 @@
         while self.check_token(pos, ["TAB", "SPACE", "NEWLINE"]) is True:
             if self.check_token(pos, "NEWLINE"):
                 pos += 1
                 break
             pos += 1
         return pos
 
-    def skip_ws(self, pos, nl=False):
+    def skip_ws(self, pos, nl=False, comment=False):
         ws = whitespaces[:]
         if nl is False:
             ws.remove("NEWLINE")
+        if comment:
+            ws += ("COMMENT", "MULT_COMMENT")
         while self.check_token(pos, ws):
             pos += 1
         return pos
 
     def skip_nest_reverse(self, pos):
         """Skips anything between two brackets, parentheses or braces starting
         at 'pos', if the brackets, parentheses or braces are not closed or
```

### Comparing `norminette-3.3.52/norminette/lexer/dictionary.py` & `norminette-3.3.53/norminette/lexer/dictionary.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,30 +35,14 @@
     "volatile": "VOLATILE",
     "while": "WHILE",
     "inline": "INLINE",
     "NULL": "NULL",
     "restrict": "RESTRICT",
 }
 
-preproc_keywords = {
-    "define": "DEFINE",
-    "error": "ERROR",
-    "endif": "ENDIF",
-    "elif": "ELIF",
-    "ifdef": "IFDEF",
-    "ifndef": "IFNDEF",
-    "if": "#IF",
-    "else": "#ELSE",
-    "include": "INCLUDE",
-    "pragma": "PRAGMA",
-    "undef": "UNDEF",
-    "warning": "WARNING",
-    "import": "IMPORT",
-}
-
 """
 __FILE__ ?add?
 __LINE__ ?add?
 __DATE__ ?add?
 __TIME__ ?add?
 __TIMESTAMP__ ?add?
 """
@@ -111,8 +95,8 @@
     "}": "RBRACE",
     "(": "LPARENTHESIS",
     ")": "RPARENTHESIS",
     "[": "LBRACKET",
     "]": "RBRACKET",
 }
 
-__all__ = ["brackets", "operators", "preproc_keywords", "keywords"]
+__all__ = ["brackets", "operators", "keywords"]
```

### Comparing `norminette-3.3.52/norminette/lexer/lexer.py` & `norminette-3.3.53/norminette/lexer/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import string
 
 from norminette.lexer.dictionary import brackets
 from norminette.lexer.dictionary import keywords
 from norminette.lexer.dictionary import operators
-from norminette.lexer.dictionary import preproc_keywords
 from norminette.lexer.tokens import Token
 
 
 def read_file(filename):
     with open(filename) as f:
         return f.read()
 
@@ -49,20 +48,15 @@
         return self.__char
 
     def pop_char(self):
         """Pop a character that's been read by increasing self.__pos,
         for escaped characters self.__pos will be increased twice
         """
         if self.peek_char() == "\t":
-            # this calculates the 'visual offset' of a tab based on it's
-            # position on the line, if there's an easier way to calculate this
-            # you're welcome
-            self.__line_pos = int(
-                (self.__line_pos + 4 - (self.__line_pos - 1) % 4) * 5 / 5
-            )
+            self.__line_pos += 4 - (self.__line_pos-1 & 3)
         else:
             self.__line_pos += 1
         if self.__pos < self.len and self.src[self.__pos] == "\\":
             self.__pos += 1
         self.__pos += 1
         return self.peek_char()
 
@@ -385,39 +379,14 @@
                 self.tokens.append(Token(operators[self.peek_char()], pos))
                 self.pop_char()
 
         else:
             self.tokens.append(Token(operators[self.src[self.__pos]], pos))
             self.pop_char()
 
-    def preprocessor(self):
-        pos = self.line_pos()
-        tkn_value = ""
-        while self.peek_char():
-            tkn_value += self.peek_char()
-            self.pop_char()
-            if self.peek_sub_string(2) == "\\\n":
-                self.__line_pos = 1
-                self.__line += 1
-            #    raise TokenError(self.line_pos())
-            if self.peek_sub_string(2) in ["//", "/*"] or self.peek_char() == "\n":
-                break
-        if len(tkn_value) <= 1:
-            raise TokenError(self.line_pos())
-        tkn_key = tkn_value[1:].split()[0]
-        if tkn_key not in preproc_keywords and tkn_key[: len("include")] != "include":
-            raise TokenError(self.line_pos())
-        else:
-            if (
-                tkn_key not in preproc_keywords
-                and tkn_key[: len("include")] == "include"
-            ):
-                tkn_key = "include"
-            self.tokens.append(Token(preproc_keywords.get(tkn_key), pos, tkn_value))
-
     def get_next_token(self):
         """Peeks one character and tries to match it to a token type,
         if it doesn't match any of the token types, an error will be raised
         and current file's parsing will stop
         """
         while self.peek_char() is not None:
             if self.is_string():
@@ -431,15 +400,16 @@
             elif self.is_constant():
                 self.constant()
 
             elif self.is_char_constant():
                 self.char_constant()
 
             elif self.peek_char() == "#":
-                self.preprocessor()
+                self.tokens.append(Token("HASH", self.line_pos()))
+                self.pop_char()
 
             elif self.src[self.__pos :].startswith("/*"):
                 self.mult_comment()
 
             elif self.src[self.__pos :].startswith("//"):
                 self.comment()
```

### Comparing `norminette-3.3.52/norminette/lexer/tokens.py` & `norminette-3.3.53/norminette/lexer/tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,18 @@
         if tkn_value is not None:
             self.value = str(tkn_value)
             self.length = len(tkn_value)
         else:
             self.value = None
             self.length = 0
 
+    @property
+    def line_column(self):
+        return self.pos[1]
+
     def __repr__(self):
         """
         Token representation for debugging, using the format <TYPE=value>
         or simply <TYPE> when value is None
         """
         r = f"<{self.type}={self.value}>" if self.value else f"<{self.type}>"
         return r
```

### Comparing `norminette-3.3.52/norminette/norm_error.py` & `norminette-3.3.53/norminette/norm_error.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 errors = {
     "SPC_INSTEAD_TAB": "Spaces at beginning of line",
     "TAB_INSTEAD_SPC": "Found tab when expecting space",
     "CONSECUTIVE_SPC": "Two or more consecutives spaces",
+    "CONSECUTIVE_WS": "Two or more consecutives white spaces",
     "SPC_BFR_OPERATOR": "missing space before operator",
     "SPC_AFTER_OPERATOR": "missing space after operator",
     "NO_SPC_BFR_OPR": "extra space before operator",
     "NO_SPC_AFR_OPR": "extra space after operator",
     "SPC_AFTER_PAR": "Missing space after parenthesis (brace/bracket)",
     "SPC_BFR_PAR": "Missing space before parenthesis (brace/bracket)",
     "NO_SPC_AFR_PAR": "Extra space after parenthesis (brace/bracket)",
@@ -22,25 +23,35 @@
     "LINE_TOO_LONG": "line too long",
     "EXP_PARENTHESIS": "Expected parenthesis",
     "MISSING_IDENTIFIER": "missing type qualifier or identifier in function arguments",
     "FORBIDDEN_CHAR_NAME": "user defined identifiers should contain only lowercase characters, \
 digits or '_'",
     "TOO_FEW_TAB": "Missing tabs for indent level",
     "TOO_MANY_TAB": "Extra tabs for indent level",
+    "TOO_MANY_WS": "Extra whitespaces for indent level",
     "SPACE_REPLACE_TAB": "Found space when expecting tab",
     "TAB_REPLACE_SPACE": "Found tab when expecting space",
     "TOO_MANY_LINES": "Function has more than 25 lines",
     "SPACE_EMPTY_LINE": "Space on empty line",
     "SPC_BEFORE_NL": "Space before newline",
     "TOO_MANY_INSTR": "Too many instructions on a single line",
+    "PREPROC_NO_SPACE": "Missing space after preprocessor directive",
     "PREPROC_UKN_STATEMENT": "Unrecognized preprocessor statement",
     "PREPROC_START_LINE": "Preprocessor statement not at the beginning of the line",
     "PREPROC_CONSTANT": "Preprocessor statement must only contain constant defines",
     "PREPROC_EXPECTED_EOL": "Expected EOL after preprocessor statement",
+    "PREPROC_BAD_IF": "If preprocessor statement without endif",
+    "PREPROC_BAD_ELIF": "Elif preprocessor statement without if or elif",
+    "PREPROC_BAD_IFDEF": "Ifdef preprocessor statement without endif",
+    "PREPROC_BAD_IFNDEF": "Ifndef preprocessor statement without endif",
+    "PREPROC_BAD_ELSE": "Else preprocessor statement without if or elif",
+    "PREPROC_BAD_ENDIF": "Endif preprocessor statement without if, elif or else",
     "PREPROC_BAD_INDENT": "Bad preprocessor indentation",
+    "PREPROC_MULTLINE": "Multiline preprocessor statement is forbidden",
+    "PREPOC_ONLY_GLOBAL": "Preprocessor statements are only allowed in the global scope",
     "USER_DEFINED_TYPEDEF": "User defined typedef must start with t_",
     "STRUCT_TYPE_NAMING": "Structure name must start with s_",
     "ENUM_TYPE_NAMING": "Enum name must start with e_",
     "UNION_TYPE_NAMING": "Union name must start with u_",
     "GLOBAL_VAR_NAMING": "Global variable must start with g_",
     "GLOBAL_VAR_DETECTED": "Global variable present in file. Make sure it is a reasonable choice.",
     "EOL_OPERATOR": "Logic operator at the end of line",
@@ -67,40 +78,47 @@
     "EXP_SEMI_COLON": "Expected semicolon",
     "EXP_TAB": "Expected tab",
     "NO_ARGS_VOID": "Empty function argument requires void",
     "MISALIGNED_VAR_DECL": "Misaligned variable declaration",
     "MISALIGNED_FUNC_DECL": "Misaligned function declaration",
     "WRONG_SCOPE_COMMENT": "Comment is invalid in this scope",
     "MACRO_NAME_CAPITAL": "Macro name must be capitalized",
+    "MACRO_FUNC_FORBIDDEN": "Macro functions are forbidden",
     "ASSIGN_IN_CONTROL": "Assignment in control structure",
     "VLA_FORBIDDEN": "Variable length array forbidden",
     "TOO_MANY_ARGS": "Function has more than 4 arguments",
     "INCLUDE_HEADER_ONLY": ".c file includes are forbidden",
     "INCLUDE_START_FILE": "Include must be at the start of file",
     "HEADER_PROT_ALL": "Header protection must include all the instructions",
+    "HEADER_PROT_ALL_AF": "Instructions after header protection are forbidden",
     "HEADER_PROT_NAME": "Wrong header protection name",
+    "HEADER_PROT_UPPER": "Header protection must be in uppercase",
+    "HEADER_PROT_MULT": "Multiple header protections, only one is allowed",
+    "HEADER_PROT_NODEF": "Header protection not containing #define",
     "TERNARY_FBIDDEN": "Ternaries are forbidden",
     "TOO_MANY_VALS": "Too many values on define",
     "NEWLINE_IN_DECL": "Newline in declaration",
     "MULT_IN_SINGLE_INSTR": "Multiple instructions in single line control structure",
     "NEWLINE_DEFINE": "Newline in define",
     "MISSING_TYPEDEF_ID": "Missing identifier in typedef declaration",
     "LABEL_FBIDDEN": "Label statements are forbidden",
+    "GOTO_FBIDDEN": "Goto statements are forbidden",
     "PREPROC_GLOBAL": "Preprocessors can only be used in the global scope",
     "WRONG_SCOPE_FCT": "Function prototype in incorrect scope",
     "WRONG_SCOPE": "Statement is in incorrect scope",
     "INCORRECT_DEFINE": "Incorrect values in define",
     "BRACE_NEWLINE": "Expected newline before brace",
     "EXP_NEWLINE": "Expected newline after control structure",
     "ARG_TYPE_UKN": "Unrecognized variable type",
     "COMMENT_ON_INSTR": "Comment must be on its own line",
     "COMMA_START_LINE": "Comma at line start",
     "MIXED_SPACE_TAB": "Mixed spaces and tabs",
     "ATTR_EOL": "Function attribute must be at the end of line",
     "INVALID_HEADER": "Missing or invalid 42 header",
+    "INCLUDE_MISSING_SP": "Missing space between include and filename",
 }
 
 
 class NormError:
     def __init__(self, errno, line, col=None):
         self.errno = errno
         self.line = line
```

### Comparing `norminette-3.3.52/norminette/registry.py` & `norminette-3.3.53/norminette/registry.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_assignation.py` & `norminette-3.3.53/norminette/rules/check_assignation.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_assignation_indent.py` & `norminette-3.3.53/norminette/rules/check_assignation_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_block_start.py` & `norminette-3.3.53/norminette/rules/check_block_start.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_brace.py` & `norminette-3.3.53/norminette/rules/check_brace.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_comment.py` & `norminette-3.3.53/norminette/rules/check_comment.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_comment_line_len.py` & `norminette-3.3.53/norminette/rules/check_comment_line_len.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_control_statement.py` & `norminette-3.3.53/norminette/rules/check_control_statement.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_declaration.py` & `norminette-3.3.53/norminette/rules/check_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_empty_line.py` & `norminette-3.3.53/norminette/rules/check_empty_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,15 @@
         No other empty lines are allowed in functions
         You must have an empty between two functions
         """
         i = 0
         if len(context.history) == 1 and context.history[-1] == "IsEmptyLine":
             context.new_error("EMPTY_LINE_FILE_START", context.peek_token(i))
             return False, 0
-        if (
-            context.scope.name != "GlobalScope"
-            and context.history[-1] != "IsBlockStart"
-        ):
+        if context.scope.name != "GlobalScope":
             if (
                 context.history[-1] != "IsVarDeclaration"
                 and context.scope.vdeclarations_allowed is True
             ):
                 context.scope.vdeclarations_allowed = False
                 if context.history[-1] not in ["IsEmptyLine", "IsComment"]:
                     if (
```

### Comparing `norminette-3.3.52/norminette/rules/check_enum_var_decl.py` & `norminette-3.3.53/norminette/rules/check_enum_var_decl.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_expression_statement.py` & `norminette-3.3.53/norminette/rules/check_expression_statement.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_func_arguments_name.py` & `norminette-3.3.53/norminette/rules/check_func_arguments_name.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_func_declaration.py` & `norminette-3.3.53/norminette/rules/check_func_declaration.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             context.check_token(i, ["RPARENTHESIS"])
         ) is True:  # , "SPACE", "TAB"])) is True:
             i += 1
         if context.check_token(i, "LPARENTHESIS") is False:
             context.new_error("EXP_PARENTHESIS", context.peek_token(i))
         i += 1
         deep = 1
-        while deep > 0:
+        while deep > 0 and context.peek_token(i) is not None:
             if context.check_token(i, "LPARENTHESIS"):
                 i = context.skip_nest(i)
             elif context.check_token(i, "RPARENTHESIS"):
                 deep -= 1
             elif context.check_token(i, "COMMA"):
                 arg += 1
             i += 1
```

### Comparing `norminette-3.3.52/norminette/rules/check_func_spacing.py` & `norminette-3.3.53/norminette/rules/check_func_spacing.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_general_spacing.py` & `norminette-3.3.53/norminette/rules/check_general_spacing.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_global_naming.py` & `norminette-3.3.53/norminette/rules/check_global_naming.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_header.py` & `norminette-3.3.53/norminette/rules/check_header.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_identifier_name.py` & `norminette-3.3.53/norminette/rules/check_identifier_name.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_in_header.py` & `norminette-3.3.53/norminette/rules/check_in_header.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,10 +48,8 @@
             return False, 0
         sc = context.scope
         while sc.name != "GlobalScope":
             sc = sc.get_outer()
         if context.history[-1] not in allowed_in_header:
             context.new_error("FORBIDDEN_IN_HEADER", context.peek_token(0))
             return False, 0
-        elif context.history[-1] in must_be_within_define and sc.header_protection != 1:
-            context.new_error("HEADER_PROT_ALL", context.peek_token(0))
         return False, 0
```

### Comparing `norminette-3.3.52/norminette/rules/check_line_count.py` & `norminette-3.3.53/norminette/rules/check_line_count.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_line_indent.py` & `norminette-3.3.53/norminette/rules/check_line_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_line_len.py` & `norminette-3.3.53/norminette/rules/check_line_len.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_many_instructions.py` & `norminette-3.3.53/norminette/rules/check_many_instructions.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_nest_line_indent.py` & `norminette-3.3.53/norminette/rules/check_nest_line_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_newline_indent.py` & `norminette-3.3.53/norminette/rules/check_newline_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_operators_spacing.py` & `norminette-3.3.53/norminette/rules/check_operators_spacing.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_preprocessor_indent.py` & `norminette-3.3.53/norminette/rules/check_preprocessor_protection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,72 @@
-from norminette.rules import Rule
+import itertools
+from pathlib import Path
 
-ALLOWED_PREPROC = [
-    "DEFINE",
-    "IFNDEF",
-    "IFDEF",
-    "#IF",
-    "ELIF",
-    "#ELSE",
-    "ENDIF",
-    "INCLUDE",
-    "WARNING",
-    "UNDEF",
-    "ERROR",
-]
-TOO_MUCH_INDENT = ["IFNDEF", "IFDEF", "ELIF", "#IF", "#ELSE"]
+from norminette.rules import Rule
 
 
-class CheckPreprocessorIndent(Rule):
+class CheckPreprocessorProtection(Rule):
     def __init__(self):
         super().__init__()
-        self.depends_on = ["IsPreprocessorStatement"]
-
-    def get_space_number(self, val):
-        val = val[1:]
-        spaces = 0
-        for i in val:
-            if i == " ":
-                spaces += 1
-            else:
-                return spaces
+        self.depends_on = [
+            "IsPreprocessorStatement",
+        ]
 
     def run(self, context):
         """
-        Preprocessor statements must be indented by an additionnal space for each #ifdef/#ifndef/#if
-        statement.
-        Structure is `#{indentation}preproc_statement`
-        Preprocessor must always be at the start of the line
+        Header protection must be as follows:
+        ```c
+        #ifndef __FILENAME_H__
+        # define __FILENAME_H__
+        #endif
+        ```
+        Any header instruction must be within the header protection
         """
-        i = 0
+        if context.filetype != "h":
+            return False, 0
+        i = context.skip_ws(0)
+        hash = context.peek_token(i)
+        i += 1  # Skip the HASH
         i = context.skip_ws(i)
-        tken = context.peek_token(i)
-        current_indent = context.preproc_scope_indent
-        if context.peek_token(i).pos[1] != 1:
-            context.new_error("PREPROC_START_LINE", context.peek_token(0))
-        tken = context.peek_token(i)
-        if context.check_token(i, ALLOWED_PREPROC) is False:
-            context.new_error("PREPROC_UKN_STATEMENT", context.peek_token(i))
-        if context.check_token(i, TOO_MUCH_INDENT) is True:
-            current_indent -= 1
-        if current_indent < 0:
-            current_indent = 0
-        spaces = self.get_space_number(tken.value if tken.value else tken.type)
-        if current_indent != spaces:
-            context.new_error("PREPROC_BAD_INDENT", context.peek_token(i))
-
+        if not context.check_token(i, "IDENTIFIER"):
+            return False, 0
+        # TODO: Add to check if macro definition is bellow #ifndef
+        t = context.peek_token(i)
+        if not t or t.type != "IDENTIFIER" or t.value.upper() not in ("IFNDEF", "ENDIF"):
+            return False, 0
         i += 1
-        tken = context.peek_token(i)
-        if tken is not None and tken.type not in ["NEWLINE", "COMMENT", "MULT_COMMENT"]:
-            context.new_error("PREPROC_EXPECTED_EOL", context.peek_token(i))
+        guard = Path(context.filename).name.upper().replace(".", "_")
+        if t.value.upper() == "ENDIF":
+            if context.preproc.indent == 0 and not context.protected:
+                i = context.skip_ws(i, nl=True, comment=True)
+                if context.peek_token(i) is not None:
+                    context.new_error("HEADER_PROT_ALL_AF", context.peek_token(i))
+                if not context.preproc.has_macro_defined(guard):
+                    context.new_error("HEADER_PROT_NODEF", hash)
+                context.protected = True
+            return False, 0
+        if context.preproc.indent != 1:
+            return False, 0
+        i = context.skip_ws(i)
+        macro = context.peek_token(i).value
+        if macro != guard and not context.protected:
+            if macro.upper() == guard:
+                context.new_error("HEADER_PROT_UPPER", context.peek_token(i))
+            else:
+                context.new_error("HEADER_PROT_NAME", context.peek_token(i))
+
+        if context.protected:
+            context.new_error("HEADER_PROT_MULT", hash)
+            return False, 0
+
+        headers = (
+            "IsComment",
+            "IsEmptyLine",
+        )
+        history = context.history[:-1]  # Remove the current `IsPreprocessorStatement`
+        history = itertools.filterfalse(lambda item: item in headers, history)
+        if next(history, None):
+            # We can't say what line contains the instruction outside
+            # header protection due to limited history information.
+            context.new_error("HEADER_PROT_ALL", hash)
+
         return False, 0
```

### Comparing `norminette-3.3.52/norminette/rules/check_preprocessor_protection.py` & `norminette-3.3.53/norminette/rules/check_preprocessor_include.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-from pathlib import Path
+import os.path
+import itertools
 
-from norminette.lexer import Lexer
 from norminette.rules import Rule
-from norminette.scope import GlobalScope
 
 
-class CheckPreprocessorProtection(Rule):
+class CheckPreprocessorInclude(Rule):
     def __init__(self):
         super().__init__()
         self.depends_on = ["IsPreprocessorStatement"]
 
     def run(self, context):
         """
-        Header protection must be as follows:
-        ```
-        #ifndef __FILENAME_H__
-        # define __FILENAME_H__
-        #endif
-        ```
-        Any header instruction must be within the header protection
+        Includes must be at the start of the file
+        You cannot include anything that isn't an header file
         """
-        i = 0
-        if type(context.scope) is not GlobalScope:
+        i = hash_index = context.skip_ws(0)
+        i += 1  # skip HASH
+        i = context.skip_ws(i)
+        if context.check_token(i, "IDENTIFIER") is False:
             return False, 0
-        if context.check_token(i, ["IFNDEF", "ENDIF"]) is False or context.filetype != "h":
+        if context.peek_token(i).value != "include":
             return False, 0
-        # protection = context.filename.upper().split("/")[-1].replace(".", "_")
-        protection = Path(context.filename).name.upper().replace(".", "_")
-        val = context.peek_token(i).value.split(" ")[-1]
-        content = Lexer(val, context.peek_token(i).pos[0])
-        tkns = content.get_tokens()
-        if context.check_token(i, "IFNDEF") is True:
-            if (
-                len(tkns) >= 1
-                and tkns[0].value == protection
-                and context.scope.header_protection == -1
-                and context.preproc_scope_indent == 1
-            ):
-                if len(context.history) > 1:
-                    for i in range(len(context.history) - 2, 0, -1):
-                        if context.history[i] != "IsEmptyLine" and context.history[i] != "IsComment":
-                            context.new_error("HEADER_PROT_ALL", context.peek_token(0))
-                            break
-                context.scope.header_protection = 0
-            elif len(tkns) < 1 or (tkns[0].value != protection and context.scope.header_protection == -1):
-                context.new_error("HEADER_PROT_NAME", context.peek_token(0))
-        elif context.check_token(i, "ENDIF") is True:
-            if context.scope.header_protection == 1 and context.preproc_scope_indent == 0:
-                context.scope.header_protection = 2
-        return False, 0
+        if not self.is_in_start_of_file(context):
+            context.new_error("INCLUDE_START_FILE", context.peek_token(hash_index))
+
+        i += 1  # skip INCLUDE
+        i = context.skip_ws(i)
+        if context.check_token(i, "STRING"):  # "niumxp.h"
+            file = context.peek_token(i).value.strip().strip('"')
+            file, extension = os.path.splitext(file)
+            if extension != ".h":
+                context.new_error("INCLUDE_HEADER_ONLY", context.peek_token(i))
+        else:  # <niumxp.h>
+            less = context.peek_token(i)
+            while not context.check_token(i, "MORE_THAN"):
+                i += 1
+            last = context.peek_token(i - 1)
+            prev = context.peek_token(i - 2)
+            if last.type != "IDENTIFIER" or not (last.value == "h" and prev.type == "DOT"):
+                context.new_error("INCLUDE_HEADER_ONLY", less)
+
+        i += 1  # skip MORE_THAN or STRING
+
+        return True, i
+
+    def is_in_start_of_file(self, context):
+        """Check if the include is at the start of the file
+        """
+        headers = (
+            "IsComment",
+            "IsEmptyLine",
+            "IsPreprocessorStatement",
+        )
+        history = itertools.filterfalse(lambda item: item in headers, context.history)
+        return (
+            context.scope.include_allowed
+            and next(history, None) is None
+        )
```

### Comparing `norminette-3.3.52/norminette/rules/check_prototype_indent.py` & `norminette-3.3.53/norminette/rules/check_prototype_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_spacing.py` & `norminette-3.3.53/norminette/rules/check_spacing.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     def run(self, context):
         """
         Indentation (except for preprocessors) must be done with tabs
         There cannot be trailing spaces or tabs at the end of line
         """
         i = 0
-        if context.history[-1] == "IsEmptyLine":
+        if context.history[-1] in ("IsEmptyLine", "IsPreprocessorStatement"):
             return False, 0
         space_tab_error = False
         space_error = False
         while i in range(len(context.tokens[: context.tkn_scope])):
             if context.check_token(i, "SPACE"):
                 if context.check_token(i - 1 if i > 0 else 0, "TAB"):
                     if space_tab_error is False:
```

### Comparing `norminette-3.3.52/norminette/rules/check_struct_naming.py` & `norminette-3.3.53/norminette/rules/check_struct_naming.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_utype_declaration.py` & `norminette-3.3.53/norminette/rules/check_utype_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_variable_declaration.py` & `norminette-3.3.53/norminette/rules/check_variable_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/check_variable_indent.py` & `norminette-3.3.53/norminette/rules/check_variable_indent.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_ambiguous_declaration.py` & `norminette-3.3.53/norminette/rules/is_ambiguous_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_assignation.py` & `norminette-3.3.53/norminette/rules/is_assignation.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_block_end.py` & `norminette-3.3.53/norminette/rules/is_block_end.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_block_start.py` & `norminette-3.3.53/norminette/rules/is_block_start.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,30 +22,33 @@
         Creates new scope based on previous instruction or set it to multiline if it
         is a control statement
         """
         i = context.skip_ws(0, nl=False)
         if context.check_token(i, "LBRACE") is False:
             return False, 0
         i += 1
-        hist = context.history
         lines = context.scope.lines
-        for item in hist[::-1]:
+        for item in reversed(context.history):
             if item == "IsEmptyLine" or item == "IsComment" or item == "IsPreprocessorStatement":
                 lines -= 1
                 continue
             if (
                 item
                 not in [
                     "IsControlStatement",
                     "IsFuncDeclaration",
                     "IsUserDefinedType",
                 ]
                 or (item in ["IsControlStatement", "IsFuncDeclaration", "IsUserDefinedType"] and lines >= 1)
             ):
-                context.sub = context.scope.inner(ControlStructure)
+                scope = {
+                    "IsFuncDeclaration": Function,
+                    "IsUserDefinedType": UserDefinedType,
+                }.get(item, ControlStructure)
+                context.sub = context.scope.inner(scope)
                 context.sub.multiline = True
                 break
             else:
                 context.scope.multiline = True
             break
 
         tmp = i
```

### Comparing `norminette-3.3.52/norminette/rules/is_cast.py` & `norminette-3.3.53/norminette/rules/is_cast.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_control_statement.py` & `norminette-3.3.53/norminette/rules/is_control_statement.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_declaration.py` & `norminette-3.3.53/norminette/rules/is_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_empty_line.py` & `norminette-3.3.53/norminette/rules/is_empty_line.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_enum_var_decl.py` & `norminette-3.3.53/norminette/rules/is_enum_var_decl.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_expression_statement.py` & `norminette-3.3.53/norminette/rules/is_expression_statement.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_func_declaration.py` & `norminette-3.3.53/norminette/rules/is_func_prototype.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-from norminette.scope import Function
 from norminette.context import GlobalScope
+from norminette.scope import UserDefinedType
 from norminette.rules import PrimaryRule
 
-
 whitespaces = ["SPACE", "TAB"]
-
-SEPARATORS = ["COMMA", "AND", "OR", "SEMI_COLON"]
-preproc = [
-    "DEFINE",
-    "ERROR",
-    "ENDIF",
-    "ELIF",
-    "IFDEF",
-    "IFNDEF",
-    "#IF",
-    "#ELSE",
-    "INCLUDE",
-    "PRAGMA",
-    "UNDEF",
-]
 assigns = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
     "ADD_ASSIGN",
     "SUB_ASSIGN",
     "MUL_ASSIGN",
     "DIV_ASSIGN",
@@ -56,22 +40,22 @@
     "UNION",
     "VOID",
     "LONG",
     "SHORT",
 ]
 
 
-class IsFuncDeclaration(PrimaryRule):
+class IsFuncPrototype(PrimaryRule):
     def __init__(self):
         super().__init__()
-        self.priority = 81
+        self.priority = 82
         self.scope = [GlobalScope]
 
     def check_args(self, context, pos):
-        i = context.skip_ws(pos, nl=True)
+        i = context.skip_ws(pos)
         while context.check_token(i, whitespaces + ["RPARENTHESIS"]):
             i += 1
         if context.check_token(i, "LPARENTHESIS") is False:
             return False, pos
         p = 1
         i += 1
         while p:
@@ -81,173 +65,157 @@
                 p -= 1
             elif context.peek_token(i) is None:
                 return False, 0
             i += 1
         return True, i
 
     def check_func_identifier(self, context, pos):
-        i = context.skip_ws(pos, nl=True)
+        i = context.skip_ws(pos)
         pp = 0  # Pointer operator's position
         lp = 0  # Left parenthesis counter (nesting level)
-
         if context.check_token(i, "IDENTIFIER"):
             i += 1
             return True, i, False
 
         d = ["LPARENTHESIS", "MULT"] + whitespaces
         while context.check_token(i, d):
             if context.check_token(i, "MULT") and not pp:
                 pp = i
             elif pp and context.check_token(i, "LPARENTHESIS"):
                 lp += 1
             i += 1
-        i = context.skip_misc_specifier(i, nl=True)
+        i = context.skip_misc_specifier(i)
         if context.check_token(i, "IDENTIFIER") is False:
             return False, pos, False
 
         i += 1
         while context.check_token(i, ["RPARENTHESIS"] + whitespaces):
             if context.check_token(i, "RPARENTHESIS"):
                 lp -= 1
             i += 1
-        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS"):
+        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS") is False:
             return False, pos, False
-
         return True, i, (True if pp else False)
 
     def check_func_format(self, context):
         i = context.skip_ws(0, nl=False)
         type_id = []
         misc_id = []
-        identifier = None
+        arg_start = 0
+        arg_end = 0
         args = False
+        identifier = None
         if context.check_token(i, "NEWLINE") is True:
             return False, 0
-        while context.peek_token(i):
+        while context.peek_token(i):  # and context.check_token(i, "NEWLINE") is False:
             while (
                 context.check_token(i, "IDENTIFIER") is True
                 and context.peek_token(i).value == "__attribute__"
             ):
                 i += 1
                 i = context.skip_ws(i)
-                i = context.skip_nest(i)
+                i = context.skip_nest(i) + 1
                 i = context.skip_ws(i)
-            if (
-                context.check_token(i, "NEWLINE") is True
-                and identifier is False
-                and misc_id == []
-                and type_id == []
-            ):
-                return False, 0
             if context.check_token(i, misc_identifier) is True:
                 misc_id.append(context.peek_token(i))
             elif context.check_token(i, type_identifier) is True:
                 type_id.append(context.peek_token(i))
             if (
                 context.check_token(
-                    i, assigns + ["TYPEDEF", "COMMA", "LBRACE"] + preproc
+                    i, assigns + ["TYPEDEF", "COMMA", "LBRACE", "RBRACE", "HASH"]
                 )
                 is True
             ):
                 return False, 0
             if context.check_token(i, "SEMI_COLON") is True:
-                return False, 0
+                break
             elif context.check_token(i, "IDENTIFIER") is True:
                 if identifier is not None:
                     type_id.append(identifier[0])
                 identifier = (context.peek_token(i), i)
-            if context.check_token(i, "NEWLINE") is True:
-                if args is False:
-                    i += 1
-                    continue
-                else:
-                    break
             if context.check_token(i, "LPARENTHESIS") is True:
                 par = context.parenthesis_contain(i)
                 if par[0] == "function":
                     if identifier is not None:
                         type_id.append(identifier[0])
                     while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
                         i += 1
                     identifier = (context.peek_token(i), i)
                     i = context.skip_nest(i)
-                elif identifier is not None:
+                elif par[0] == "pointer":
+                    if identifier is not None:
+                        type_id.append(identifier[0])
+                    while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
+                        i += 1
+                    identifier = (context.peek_token(i), i)
+                    nxt = par[1] + 1
+                    if context.check_token(nxt, ["LPARENTHESIS"]) is False:
+                        return False, 0
+                    i = context.skip_nest(i)
+                else:
                     args = True
                     arg_start = i
                     i = context.skip_nest(i)
                     arg_end = i
-                    while (context.check_token(i, "RPARENTHESIS")) is True:
-                        i += 1
-                    i = context.skip_ws(i)
-                    if context.check_token(i, "LPARENTHESIS") is True:
-                        arg_start = i
-                        i = context.skip_nest(i)
-                        arg_end = i
                     break
-                else:
-                    i += 1
             else:
                 i += 1
         if len(type_id) > 0 and args is True and identifier is not None:
             i = identifier[1]
-            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]) is True:
                 i += 1
             sc = context.scope
             while type(sc) != GlobalScope:
                 sc = sc.outer()
             sc.fnames.append(context.peek_token(i).value)
+            if context.func_alignment == 0:
+                tmp = i
+                while context.check_token(
+                    tmp - 1, ["LPARENTHESIS", "MULT", "BWISE_AND"]
+                ):
+                    tmp -= 1
+                context.func_alignment = int(context.peek_token(tmp).pos[1] / 4)
             context.fname_pos = i
             context.arg_pos = [arg_start, arg_end]
             i = arg_end
-            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["RPARENTHESIS"]) is True:
                 i += 1
-            i = context.skip_ws(i, nl=True)
-            if context.check_token(i, "LPARENTHESIS") is True:
-                i = context.skip_nest(i)
+            i = context.skip_nest(i)
+            while context.check_token(i, ["RPARENTHESIS"]) is True:
                 i += 1
             i = context.skip_ws(i, nl=True)
-            while context.check_token(i, "LBRACKET"):
-                i = context.skip_nest(i)
-                i += 1
-                i = context.skip_ws(i, nl=True)
-            while (
-                context.check_token(i, "IDENTIFIER") is True
-                and context.peek_token(i).value == "__attribute__"
-            ):
-                i += 1
-                i = context.skip_ws(i)
-                i = context.skip_nest(i) + 1
-                i = context.skip_ws(i)
             return True, i
         return False, 0
 
     def run(self, context):
         """
-        Catches function declaration
+        Catches function prototypes
         Allows newline inside it
-        Creates context variable for function name, arg_start, arg_end
+        End condition is SEMI_COLON token, otherwise line will be considered as
+        function declaration
         """
-        if type(context.scope) is not GlobalScope:
+        if (
+            type(context.scope) is not GlobalScope
+            and type(context.scope) is not UserDefinedType
+        ):
             return False, 0
         ret, read = self.check_func_format(context)
         if ret is False:
             return False, 0
+        if context.check_token(read, "IDENTIFIER") is True:
+            while context.peek_token(read).value == "__attribute__":
+                read += 1
+                read = context.skip_ws(read)
+                read = context.skip_nest(read) + 1
+                read = context.skip_ws(read, nl=True)
         while context.check_token(read, ["COMMENT", "MULT_COMMENT"]) is True:
             read += 1
         read = context.skip_ws(read, nl=False)
-        if context.check_token(read, ["NEWLINE", "LBRACE"] + preproc):
-            if context.check_token(read, ["LBRACE"] + preproc) is True:
-                read -= 1
-            context.scope.functions += 1
-            read += 1
-            context.sub = context.scope.inner(Function)
-            read = context.eol(read)
-            return True, read
+        if context.check_token(read, "NEWLINE"):
+            return False, 0
 
-        elif context.check_token(read, SEPARATORS):
+        elif context.check_token(read, "SEMI_COLON"):
             read += 1
             read = context.eol(read)
-            return False, 0
+            return True, read
 
         return False, 0
```

### Comparing `norminette-3.3.52/norminette/rules/is_func_prototype.py` & `norminette-3.3.53/norminette/rules/is_func_declaration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,15 @@
+from norminette.scope import Function
 from norminette.context import GlobalScope
-from norminette.scope import UserDefinedType
 from norminette.rules import PrimaryRule
 
+
 whitespaces = ["SPACE", "TAB"]
-preproc = [
-    "DEFINE",
-    "ERROR",
-    "ENDIF",
-    "ELIF",
-    "IFDEF",
-    "IFNDEF",
-    "#IF",
-    "#ELSE",
-    "INCLUDE",
-    "PRAGMA",
-    "UNDEF",
-]
+
+SEPARATORS = ["COMMA", "AND", "OR", "SEMI_COLON"]
 assigns = [
     "RIGHT_ASSIGN",
     "LEFT_ASSIGN",
     "ADD_ASSIGN",
     "SUB_ASSIGN",
     "MUL_ASSIGN",
     "DIV_ASSIGN",
@@ -53,22 +43,22 @@
     "UNION",
     "VOID",
     "LONG",
     "SHORT",
 ]
 
 
-class IsFuncPrototype(PrimaryRule):
+class IsFuncDeclaration(PrimaryRule):
     def __init__(self):
         super().__init__()
-        self.priority = 82
+        self.priority = 81
         self.scope = [GlobalScope]
 
     def check_args(self, context, pos):
-        i = context.skip_ws(pos)
+        i = context.skip_ws(pos, nl=True)
         while context.check_token(i, whitespaces + ["RPARENTHESIS"]):
             i += 1
         if context.check_token(i, "LPARENTHESIS") is False:
             return False, pos
         p = 1
         i += 1
         while p:
@@ -78,157 +68,175 @@
                 p -= 1
             elif context.peek_token(i) is None:
                 return False, 0
             i += 1
         return True, i
 
     def check_func_identifier(self, context, pos):
-        i = context.skip_ws(pos)
+        i = context.skip_ws(pos, nl=True)
         pp = 0  # Pointer operator's position
         lp = 0  # Left parenthesis counter (nesting level)
+
         if context.check_token(i, "IDENTIFIER"):
             i += 1
             return True, i, False
 
         d = ["LPARENTHESIS", "MULT"] + whitespaces
         while context.check_token(i, d):
             if context.check_token(i, "MULT") and not pp:
                 pp = i
             elif pp and context.check_token(i, "LPARENTHESIS"):
                 lp += 1
             i += 1
-        i = context.skip_misc_specifier(i)
+        i = context.skip_misc_specifier(i, nl=True)
         if context.check_token(i, "IDENTIFIER") is False:
             return False, pos, False
 
         i += 1
         while context.check_token(i, ["RPARENTHESIS"] + whitespaces):
             if context.check_token(i, "RPARENTHESIS"):
                 lp -= 1
             i += 1
-        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS") is False:
+        if pp and lp < 0 and context.check_token(i, "LPARENTHESIS"):
             return False, pos, False
+
         return True, i, (True if pp else False)
 
     def check_func_format(self, context):
         i = context.skip_ws(0, nl=False)
         type_id = []
         misc_id = []
-        arg_start = 0
-        arg_end = 0
-        args = False
         identifier = None
+        args = False
         if context.check_token(i, "NEWLINE") is True:
             return False, 0
-        while context.peek_token(i):  # and context.check_token(i, "NEWLINE") is False:
+        while context.peek_token(i):
             while (
                 context.check_token(i, "IDENTIFIER") is True
                 and context.peek_token(i).value == "__attribute__"
             ):
                 i += 1
                 i = context.skip_ws(i)
-                i = context.skip_nest(i) + 1
+                i = context.skip_nest(i)
                 i = context.skip_ws(i)
+            if (
+                context.check_token(i, "NEWLINE") is True
+                and identifier is False
+                and misc_id == []
+                and type_id == []
+            ):
+                return False, 0
             if context.check_token(i, misc_identifier) is True:
                 misc_id.append(context.peek_token(i))
             elif context.check_token(i, type_identifier) is True:
                 type_id.append(context.peek_token(i))
             if (
                 context.check_token(
-                    i, assigns + ["TYPEDEF", "COMMA", "LBRACE", "RBRACE"] + preproc
+                    i, assigns + ["TYPEDEF", "COMMA", "LBRACE", "HASH"]
                 )
                 is True
             ):
                 return False, 0
             if context.check_token(i, "SEMI_COLON") is True:
-                break
+                return False, 0
             elif context.check_token(i, "IDENTIFIER") is True:
                 if identifier is not None:
                     type_id.append(identifier[0])
                 identifier = (context.peek_token(i), i)
+            if context.check_token(i, "NEWLINE") is True:
+                if args is False:
+                    i += 1
+                    continue
+                else:
+                    break
             if context.check_token(i, "LPARENTHESIS") is True:
                 par = context.parenthesis_contain(i)
                 if par[0] == "function":
                     if identifier is not None:
                         type_id.append(identifier[0])
                     while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
                         i += 1
                     identifier = (context.peek_token(i), i)
                     i = context.skip_nest(i)
-                elif par[0] == "pointer":
-                    if identifier is not None:
-                        type_id.append(identifier[0])
-                    while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]):
-                        i += 1
-                    identifier = (context.peek_token(i), i)
-                    nxt = par[1] + 1
-                    if context.check_token(nxt, ["LPARENTHESIS"]) is False:
-                        return False, 0
-                    i = context.skip_nest(i)
-                else:
+                elif identifier is not None:
                     args = True
                     arg_start = i
                     i = context.skip_nest(i)
                     arg_end = i
+                    while (context.check_token(i, "RPARENTHESIS")) is True:
+                        i += 1
+                    i = context.skip_ws(i)
+                    if context.check_token(i, "LPARENTHESIS") is True:
+                        arg_start = i
+                        i = context.skip_nest(i)
+                        arg_end = i
                     break
+                else:
+                    i += 1
             else:
                 i += 1
         if len(type_id) > 0 and args is True and identifier is not None:
             i = identifier[1]
+            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["LPARENTHESIS", "MULT", "BWISE_AND"]) is True:
                 i += 1
             sc = context.scope
             while type(sc) != GlobalScope:
                 sc = sc.outer()
             sc.fnames.append(context.peek_token(i).value)
-            if context.func_alignment == 0:
-                tmp = i
-                while context.check_token(
-                    tmp - 1, ["LPARENTHESIS", "MULT", "BWISE_AND"]
-                ):
-                    tmp -= 1
-                context.func_alignment = int(context.peek_token(tmp).pos[1] / 4)
             context.fname_pos = i
             context.arg_pos = [arg_start, arg_end]
             i = arg_end
+            i = context.skip_ws(i, nl=True)
             while context.check_token(i, ["RPARENTHESIS"]) is True:
                 i += 1
-            i = context.skip_nest(i)
-            while context.check_token(i, ["RPARENTHESIS"]) is True:
+            i = context.skip_ws(i, nl=True)
+            if context.check_token(i, "LPARENTHESIS") is True:
+                i = context.skip_nest(i)
                 i += 1
             i = context.skip_ws(i, nl=True)
+            while context.check_token(i, "LBRACKET"):
+                i = context.skip_nest(i)
+                i += 1
+                i = context.skip_ws(i, nl=True)
+            while (
+                context.check_token(i, "IDENTIFIER") is True
+                and context.peek_token(i).value == "__attribute__"
+            ):
+                i += 1
+                i = context.skip_ws(i)
+                i = context.skip_nest(i) + 1
+                i = context.skip_ws(i)
             return True, i
         return False, 0
 
     def run(self, context):
         """
-        Catches function prototypes
+        Catches function declaration
         Allows newline inside it
-        End condition is SEMI_COLON token, otherwise line will be considered as
-        function declaration
+        Creates context variable for function name, arg_start, arg_end
         """
-        if (
-            type(context.scope) is not GlobalScope
-            and type(context.scope) is not UserDefinedType
-        ):
+        if type(context.scope) is not GlobalScope:
             return False, 0
         ret, read = self.check_func_format(context)
         if ret is False:
             return False, 0
-        if context.check_token(read, "IDENTIFIER") is True:
-            while context.peek_token(read).value == "__attribute__":
-                read += 1
-                read = context.skip_ws(read)
-                read = context.skip_nest(read) + 1
-                read = context.skip_ws(read, nl=True)
         while context.check_token(read, ["COMMENT", "MULT_COMMENT"]) is True:
             read += 1
         read = context.skip_ws(read, nl=False)
-        if context.check_token(read, "NEWLINE"):
-            return False, 0
-
-        elif context.check_token(read, "SEMI_COLON"):
+        if context.check_token(read, ["NEWLINE", "LBRACE", "HASH"]):
+            if context.check_token(read, ["LBRACE", "HASH"]) is True:
+                read -= 1
+            context.scope.functions += 1
             read += 1
+            temp = context.skip_ws(read, nl=True)
+            if context.check_token(temp, "LBRACE"):
+                context.sub = context.scope.inner(Function)
             read = context.eol(read)
             return True, read
 
+        elif context.check_token(read, SEPARATORS):
+            read += 1
+            read = context.eol(read)
+            return False, 0
+
         return False, 0
```

### Comparing `norminette-3.3.52/norminette/rules/is_function_call.py` & `norminette-3.3.53/norminette/rules/is_function_call.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_label.py` & `norminette-3.3.53/norminette/rules/is_label.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     def run(self, context):
         """
         Catches label and raises norm error whenever
         """
         i = context.skip_ws(0)
         if context.check_token(i, "IDENTIFIER") is False:
             return False, 0
-        i += 1
-        i = context.skip_ws(i)
+        i = context.skip_ws(i + 1)  # +1 to skip the identifier
         if context.check_token(i, "COLON") is False:
             return False, 0
-        while context.peek_token(i) and context.check_token(i, "NEWLINE") is False:
+        i = context.skip_ws(i + 1)  # +1 to skip the colon
+        if context.check_token(i, "NEWLINE"):
+            return True, i+1
+        while context.peek_token(i) and context.check_token(i, "SEMI_COLON") is False:
             i += 1
-        i = context.eol(i)
+        i = context.eol(i + 1)  # +1 to skip the semi-colon
         return True, i
```

### Comparing `norminette-3.3.52/norminette/rules/is_ternary.py` & `norminette-3.3.53/norminette/rules/is_ternary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from norminette.rules import Rule
+from norminette.rules import PrimaryRule
 
 
-class IsTernary(Rule):
+class IsTernary(PrimaryRule):
     def __init__(self):
         super().__init__()
         self.priority = 53
         self.scope = []
 
     def run(self, context):
         """
```

### Comparing `norminette-3.3.52/norminette/rules/is_user_defined_type.py` & `norminette-3.3.53/norminette/rules/is_user_defined_type.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/is_var_declaration.py` & `norminette-3.3.53/norminette/rules/is_var_declaration.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/rules/rule.py` & `norminette-3.3.53/norminette/rules/rule.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/scope.py` & `norminette-3.3.53/norminette/scope.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/norminette/tools/colors.py` & `norminette-3.3.53/norminette/tools/colors.py`

 * *Files identical despite different names*

### Comparing `norminette-3.3.52/pyproject.toml` & `norminette-3.3.53/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "norminette"
-version = "3.3.52"
+version = "3.3.53"
 description = "Open source C files linter for 42 Network campuses"
 authors = ["42 <pedago@42.fr>"]
 license = "MIT Licence"
 readme = "README.md"
 repository = "https://github.com/42School/norminette"
 keywords = ['42', 'norminette']
 classifiers = [
```

### Comparing `norminette-3.3.52/PKG-INFO` & `norminette-3.3.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norminette
-Version: 3.3.52
+Version: 3.3.53
 Summary: Open source C files linter for 42 Network campuses
 Home-page: https://github.com/42School/norminette
 License: MIT Licence
 Keywords: 42,norminette
 Author: 42
 Author-email: pedago@42.fr
 Requires-Python: >=3.8.1,<4.0.0
```

