# Comparing `tmp/smoldyn-2.72.dev202307112341-cp39-cp39-macosx_11_0_x86_64.whl.zip` & `tmp/smoldyn-2.72.dev202307112342-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,18 @@
-Zip file size: 1668385 bytes, number of entries: 20
--rw-r--r--  2.0 unx    78575 b- defN 23-Jul-11 23:43 smoldyn/smoldyn.py
--rw-r--r--  2.0 unx      218 b- defN 23-Jul-11 23:43 smoldyn/__init__.py
--rw-r--r--  2.0 unx     1155 b- defN 23-Jul-11 23:43 smoldyn/types.py
--rw-r--r--  2.0 unx     1098 b- defN 23-Jul-11 23:43 smoldyn/utils.py
--rwxr-xr-x  2.0 unx  1923696 b- defN 23-Jul-11 23:46 smoldyn/_smoldyn.cpython-39-darwin.so
--rw-r--r--  2.0 unx      841 b- defN 23-Jul-11 23:43 smoldyn/__main__.py
--rw-r--r--  2.0 unx    47576 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/combine.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/_version.py
--rw-r--r--  2.0 unx      489 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/__init__.py
--rw-r--r--  2.0 unx     5274 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/data_model.py
--rw-r--r--  2.0 unx    17016 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/utils.py
--rw-r--r--  2.0 unx      579 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/__main__.py
--r--r--r--  2.0 unx   201664 b- defN 23-Jul-11 23:46 smoldyn/.dylibs/liblzma.5.dylib
--r--r--r--  2.0 unx   867440 b- defN 23-Jul-11 23:46 smoldyn/.dylibs/libzstd.1.5.5.dylib
--r--r--r--  2.0 unx   538560 b- defN 23-Jul-11 23:46 smoldyn/.dylibs/libtiff.6.dylib
--r--r--r--  2.0 unx   689760 b- defN 23-Jul-11 23:46 smoldyn/.dylibs/libjpeg.8.2.2.dylib
--rw-rw-r--  2.0 unx     1751 b- defN 23-Jul-11 23:46 smoldyn-2.72.dev202307112341.dist-info/RECORD
--rw-r--r--  2.0 unx      109 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112341.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112341.dist-info/top_level.txt
--rw-r--r--  2.0 unx     2856 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112341.dist-info/METADATA
-20 files, 4378711 bytes uncompressed, 1665561 bytes compressed:  62.0%
+Zip file size: 869298 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      227 b- defN 23-Jul-11 23:43 smoldyn/__init__.py
+-rw-rw-rw-  2.0 fat      868 b- defN 23-Jul-11 23:43 smoldyn/__main__.py
+-rw-rw-rw-  2.0 fat  1925632 b- defN 23-Jul-11 23:43 smoldyn/_smoldyn.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    80975 b- defN 23-Jul-11 23:43 smoldyn/smoldyn.py
+-rw-rw-rw-  2.0 fat     1193 b- defN 23-Jul-11 23:43 smoldyn/types.py
+-rw-rw-rw-  2.0 fat     1141 b- defN 23-Jul-11 23:43 smoldyn/utils.py
+-rw-rw-rw-  2.0 fat      510 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/__init__.py
+-rw-rw-rw-  2.0 fat      605 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/__main__.py
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/_version.py
+-rw-rw-rw-  2.0 fat    48535 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/combine.py
+-rw-rw-rw-  2.0 fat     5443 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/data_model.py
+-rw-rw-rw-  2.0 fat    17365 b- defN 23-Jul-11 23:43 smoldyn/biosimulators/utils.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112342.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112342.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112342.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1361 b- defN 23-Jul-11 23:43 smoldyn-2.72.dev202307112342.dist-info/RECORD
+16 files, 2086941 bytes uncompressed, 867046 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,61 +1,49 @@
-Filename: smoldyn/smoldyn.py
-Comment: 
-
 Filename: smoldyn/__init__.py
 Comment: 
 
-Filename: smoldyn/types.py
-Comment: 
-
-Filename: smoldyn/utils.py
-Comment: 
-
-Filename: smoldyn/_smoldyn.cpython-39-darwin.so
-Comment: 
-
 Filename: smoldyn/__main__.py
 Comment: 
 
-Filename: smoldyn/biosimulators/combine.py
+Filename: smoldyn/_smoldyn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: smoldyn/biosimulators/_version.py
+Filename: smoldyn/smoldyn.py
 Comment: 
 
-Filename: smoldyn/biosimulators/__init__.py
+Filename: smoldyn/types.py
 Comment: 
 
-Filename: smoldyn/biosimulators/data_model.py
+Filename: smoldyn/utils.py
 Comment: 
 
-Filename: smoldyn/biosimulators/utils.py
+Filename: smoldyn/biosimulators/__init__.py
 Comment: 
 
 Filename: smoldyn/biosimulators/__main__.py
 Comment: 
 
-Filename: smoldyn/.dylibs/liblzma.5.dylib
+Filename: smoldyn/biosimulators/_version.py
 Comment: 
 
-Filename: smoldyn/.dylibs/libzstd.1.5.5.dylib
+Filename: smoldyn/biosimulators/combine.py
 Comment: 
 
-Filename: smoldyn/.dylibs/libtiff.6.dylib
+Filename: smoldyn/biosimulators/data_model.py
 Comment: 
 
-Filename: smoldyn/.dylibs/libjpeg.8.2.2.dylib
+Filename: smoldyn/biosimulators/utils.py
 Comment: 
 
-Filename: smoldyn-2.72.dev202307112341.dist-info/RECORD
+Filename: smoldyn-2.72.dev202307112342.dist-info/METADATA
 Comment: 
 
-Filename: smoldyn-2.72.dev202307112341.dist-info/WHEEL
+Filename: smoldyn-2.72.dev202307112342.dist-info/WHEEL
 Comment: 
 
-Filename: smoldyn-2.72.dev202307112341.dist-info/top_level.txt
+Filename: smoldyn-2.72.dev202307112342.dist-info/top_level.txt
 Comment: 
 
-Filename: smoldyn-2.72.dev202307112341.dist-info/METADATA
+Filename: smoldyn-2.72.dev202307112342.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smoldyn/smoldyn.py

 * *Ordering differences only*

```diff
@@ -1,2400 +1,2400 @@
-"""Smoldyn user API.
-"""
-
-__author__ = "Dilawar Singh"
-__email__ = "dilawar.s.rajput@gmail.com"
-
-__all__ = [
-    "__version__",
-    "version",
-    "getError",
-    "Simulation",
-    "Species",
-    "Panel",
-    "Triangle",
-    "Rectangle",
-    "Sphere",
-    "Hemisphere",
-    "Cylinder",
-    "Disk",
-    "Path2D",
-    "Surface",
-    "Port",
-    "Partition",
-    "Compartment",
-    "Reaction",
-    "BidirectionalReaction",
-]
-
-import operator
-import functools
-import math
-import warnings
-from pathlib import Path
-from dataclasses import dataclass
-
-from typing import Union, Tuple, List, Dict, Optional, Sequence
-
-
-from smoldyn.types import Color, BoundType, ColorType, DiffConst
-from smoldyn import _smoldyn
-
-# Path of model file.
-# It does not look like there is a beter way to find this path out
-# automatically. This is needed by simptr.
-import inspect
-
-__top_model_file__ = Path(inspect.stack()[-1].filename)
-
-# Logger
-import logging
-
-__logger__ = logging.getLogger(__name__)
-ch = logging.StreamHandler()
-ch.setLevel(logging.WARNING)
-ch.setFormatter(logging.Formatter("%(name)s - %(levelname)s - %(message)s"))
-__logger__.addHandler(ch)
-
-
-def version():
-    """Get version"""
-    return _smoldyn.__version__
-
-
-# alias of version()
-__version__: str = version()
-
-
-def getError(clear: bool = False) -> Tuple[_smoldyn.ErrorCode, str]:
-    return _smoldyn.getError(clear)
-
-
-def _toMS(st: Union[str, _smoldyn.MolecState]) -> _smoldyn.MolecState:
-    """Convert a string to equivalent MolecState.
-
-    Parameters
-    ----------
-    st : Tuple[str, _smoldyn.MolecState]
-        Given state either a string or MolecState. If MolecState is given, this
-        function simply returns it.
-    """
-    return _smoldyn.MolecState.__members__[st] if isinstance(st, str) else st
-
-
-class Species(object):
-    def __init__(
-        self,
-        simulation: _smoldyn.Simulation,
-        name: str,
-        state: str = "soln",
-        color: Union[ColorType, Dict[str, ColorType]] = {"soln": "black"},
-        difc: Union[float, Dict[str, float]] = 0.0,
-        display_size: float = 3,
-        mol_list: str = "",
-    ):
-        """
-        Species or Molecule.
-
-        Parameters
-        ----------
-        name : str
-            Name of the species.
-        state : str
-            State of the species. One of the following:
-                'soln', 'front', 'back', 'up', 'down', 'bsoln', 'all', 'none','some'
-        color: Color or dict of Colors
-            If a single :py:class:`Color` is given, all states of this molecule will be
-            assigned this color. To assign different colors to different
-            states, use a dictionary of :py:class:`Color`.
-        difc : float or a dict of floats
-            Diffusion coefficient. If a single value is given, all states of
-            the molecule gets the same value. To assign different values to
-            different states, use a dict e.g. {'soln':1, 'front':2}.
-        display_size : float, optional
-            display size of the molecule. For the ``opengl`` graphics method, the
-            this value is in pixels.  Here, numbers from 2 to 4 are
-            typically good choices (default 3px).  For better graphics
-            options (opengl_good and opengl_better), the display size value is
-            the radius with which the molecule is drawn, using the same units
-            as elsewhere in the input file.
-        mol_list : str, optional
-            molecule list (default '')
-
-        """
-        self.simulation = simulation
-        self.name: str = name
-        assert self.name
-
-        self._displaySize: Dict[str, float] = {}
-        self._color: Dict[str, Color] = {}
-        self._difc: Dict[str, float] = {}
-        self._mol_list: str = ""
-
-        k = self.simulation.addSpecies(self.name)
-        assert k == _smoldyn.ErrorCode.ok, f"Failed to add molecule {k}"
-
-        if state not in _smoldyn.MolecState.__members__:
-            raise NameError(
-                f"{state} is not a valid MolecState. Available "
-                "states are:{', '.join(_smoldyn.MolecState.__members__.keys())}"
-            )
-
-        self.state = state
-
-        # Prepare diffusion constant dict (for state).
-        if not isinstance(difc, dict):
-            difc = {self.state: difc}
-        self.difc = difc
-
-        # assign color
-        self.color = color
-        self.display_size = display_size
-        if mol_list:
-            self.mol_list: str = mol_list
-
-    def __repr__(self):
-        return f"<Molecule: {self.name}, difc={self.difc}, state={self.state}>"
-
-    def __to_disp__(self):
-        return f"{self.name}({self.state})"
-
-    def setStyle(
-        self,
-        display_size: Union[float, Dict[str, float]],
-        color: Union[ColorType, Dict[str, ColorType]],
-    ):
-        self.color = color
-        self.display_size = display_size
-
-    @property
-    def difc(self) -> DiffConst:
-        return self._difc
-
-    @difc.setter
-    def difc(self, difconst: DiffConst):
-        """Isotropic Diffusion coeffiecient of the Species.
-
-        Parameters
-        ----------
-        difconst : DiffConst (default '0')
-            If a single value is given, all states of the
-            molecule are assigned the same value. To assign state specific
-            values, use a dictionary. Missing states will be assigned 0.0.
-        """
-        self._difc = (
-            {self.state: difconst} if not isinstance(difconst, dict) else difconst
-        )
-        for state, D in self._difc.items():
-            st = (
-                _smoldyn.MolecState.__members__[state]
-                if isinstance(state, str)
-                else state
-            )
-            k = self.simulation.setSpeciesMobility(self.name, st, D)
-            assert k == _smoldyn.ErrorCode.ok
-
-    @property
-    def mol_list(self) -> str:
-        return self._mol_list
-
-    @mol_list.setter
-    def mol_list(self, val):
-        k = self.simulation.addMolList(val)
-        assert k == _smoldyn.ErrorCode.ok, f"Failed to add mollist: {k}"
-        k = self.simulation.setMolList(self.name, _toMS(self.state), val)
-        assert (
-            k == _smoldyn.ErrorCode.ok
-        ), f"Failed to set mol_list={val} on {self}: {k}"
-        self._mol_list = val
-
-    @property
-    def color(self):
-        return self._color
-
-    @color.setter
-    def color(self, clr: Union[ColorType, Color]):
-        self._color = {self.state: Color(clr)} if not isinstance(clr, dict) else clr
-        for state, _clr in self._color.items():
-            k = self.simulation.setMoleculeColor(
-                self.name, _toMS(state), Color(_clr).rgba
-            )
-            assert k == _smoldyn.ErrorCode.ok
-
-    @property
-    def display_size(self):
-        return self._displaySize
-
-    @display_size.setter
-    def display_size(self, size: Union[float, Dict[str, float]]):
-        """Set the display_size of the molecule.
-
-        Parameters
-        ----------
-        size : Union[float, Dict[str, float]]
-            If a single value is provided, it is applied to all states of the
-            moelcule. For state specific value of display_size, use a
-            dictionary.
-
-        Note
-        -----
-        For the “opengl” graphics level, the display size value is in pixels.
-        Here, numbers from 2 to 4 are typically good choices (deafult 2px).
-        For the two better graphics options, the display size value is the
-        radius with which the molecule is drawn, using the same units as
-        elsewhere in the input file.
-        """
-        if isinstance(size, (float, int)):
-            size = {_smoldyn.MolecState.all: size}
-        self._displaySize = size
-        for state, size in self._displaySize.items():
-            state = (
-                _smoldyn.MolecState.__members__[state]
-                if isinstance(state, str)
-                else state
-            )
-            k = self.simulation.setMoleculeSize(self.name, state, size)
-            assert k == _smoldyn.ErrorCode.ok
-
-    def addToSolution(
-        self,
-        N: int,
-        pos: List[float] = [],
-        highpos: List[float] = [],
-        lowpos: List[float] = [],
-    ):
-        """Add molecule to solution.
-
-        Parameters
-        ----------
-        N : float
-            Number of molecules
-        pos : List[float]
-            Fixed location. If given, both `lowpos` and `highpos` will be set
-            to this value.
-        highpos : List[float]
-            Upper bound on the molecules location. Molecules will be distributed
-            uniformly between the lowerbound and this value.
-        lowpos : List[float]
-            Lower bound on the molecules location. Molecules will be distributed
-            uniformly between the upper bound and this value.
-        """
-        assert (
-            self.state == "soln"
-        ), f"You can't use this function on a Species with type {self.state}"
-        if pos:
-            lowpos = highpos = pos
-        k = self.simulation.addSolutionMolecules(self.name, N, lowpos, highpos)
-        assert k == _smoldyn.ErrorCode.ok, f"Failed to add to solution: {k}"
-
-
-@dataclass
-class NullSpecies(Species):
-    name: str = ""
-    state = _smoldyn.MolecState.__members__["none"]
-
-    def __bool__(self):
-        return False
-
-    def __len__(self):
-        return 0
-
-
-# Type of a substract and product of a Reaction
-SpeciesState = Union[_smoldyn.MolecState, str]
-SpeciesWithState = Union[Species, Tuple[Species, SpeciesState]]
-
-
-class Panel(object):
-    def __init__(
-        self,
-        *,
-        name: str = "",
-        shape: _smoldyn.PanelShape = _smoldyn.PanelShape.none,
-        neighbors: List["Panel"] = [],
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Panels are components of a surface. One or more Panels are requried
-        to form a Surface. Following geometric primitives are available.
-
-        - [Rectangle](smoldyn.smoldyn.Rectangle)
-        - [Triangle](smoldyn.smoldyn.Triangle)
-        - [Sphere](smoldyn.smoldyn.Sphere)
-        - [Hemisphere](smoldyn.smoldyn.Hemisphere)
-        - [Cylinder](smoldyn.smoldyn.Cylinder)
-        - [Disk](smoldyn.smoldyn.Disk)
-        """
-
-        # self._neighbors: List[Panel] = []
-        self._neighbors: List = []
-        self.name = name
-        self.ctype: _smoldyn.PanelShape = shape
-        self.pts: List[float] = []
-        self.simulation = simulation
-        self.front = _PanelFace(name="front", panel=self, simulation=self.simulation)
-        self.back = _PanelFace(simulation=self.simulation, name="back", panel=self)
-        self.surface: Surface = NullSurface()
-        self.neighbors = neighbors
-
-    def _setSimulation(self, simulation: _smoldyn.Simulation):
-        assert simulation
-        self.simulation = simulation
-        self.front.simulation = simulation
-        self.back.simulation = simulation
-
-    def jumpTo(self, face1: str, panel2, face2: str, bidirectional: bool = False):
-        """Add a jump reaction between two panels of the same surface.
-
-        This panel has name panel1, and face face1.  A molecule that hits this
-        face of the panel, and that has “jump” action for this face, gets
-        translated to the face face2 of the panel panel2 (which needs to be the
-        same shape as the originating panel).
-
-        Parameters
-        ----------
-        face1 : Panel
-
-        panel2 : to this Panel
-        face2 : to this face
-
-        Examples
-        --------
-
-        Smoldyn expression:
-            jump r1 front <-> r2 front
-
-        >>> r1.addJump('front', r2, 'front', True)
-
-        Or,
-
-        >>> r1.front.jumpTo(r2.front, True)
-        """
-        jfrom = getattr(self, face1)
-        assert jfrom, f"Could not locate {face1} on {self}."
-        assert isinstance(jfrom, _PanelFace)
-        jto = getattr(panel2, face2)
-        assert jto, f"Could not locate {face2} on {panel2}."
-        assert isinstance(jto, _PanelFace)
-
-        return jfrom.jumpTo(jto, bidirectional)
-
-    def __str__(self):
-        return f"<{self.name} type={self.ctype} index={self.index} points={self.pts}>"
-
-    def _axisIndex(self, axisname: str):
-        axisDict = dict(x=0, y=1, z=2)
-        return int(axisDict.get(axisname.lower(), axisname))
-
-    @property
-    def index(self) -> int:
-        assert self.simulation
-        v: int = self.simulation.getPanelIndexNT(self.surface.name, self.name)
-        return v
-
-    def toText(self):
-        return f"panel {self.ctype} {self.axisstr} {' '.join(map(str,self.pts))} {self.name}".strip()
-
-    @property
-    def neighbors(self):
-        return self._neighbors
-
-    @neighbors.setter
-    def neighbors(self, panels: List):
-        self._neighbors = panels
-        for panel in panels:
-            self._assignNeighbor(panel)
-
-    @property
-    def neighbor(self):
-        return self._neighbors[0]
-
-    @neighbor.setter
-    def neighbor(self, panel):
-        self._assignNeighbor(panel)
-
-    def _assignNeighbor(self, panel, reciprocal: bool = False):
-        assert self.surface, f"Panel {self} has no Surface assigned."
-        assert panel.surface, f"Panel {panel} has no Surface assigned."
-        assert self != panel, "A panel cannot be its own neighbor"
-        assert self.simulation
-        k = self.simulation.addPanelNeighbor(
-            self.surface.name, self.name, panel.surface.name, panel.name, reciprocal
-        )
-        assert k == _smoldyn.ErrorCode.ok
-
-    def _getName(self, index: int) -> str:
-        if self.name:
-            return self.name
-        return f"{self.ctype}{index}"
-
-    def setNeighbors(self, panels, reciprocal: bool = False):
-        """Set neighbors.
-
-        Parameters
-        ----------
-        panels :
-            Neighboring panels
-        reciprocal : bool
-            If True, this panel also becomes neighbor of all panels in arguments.
-
-        See Also
-        --------
-        Panel.neighbor, Panel.neighbors
-        """
-        for panel in panels:
-            self._assignNeighbor(panel, reciprocal)
-
-
-class Rectangle(Panel):
-    def __init__(
-        self,
-        corner: Sequence[float],
-        dimensions: Sequence[float],
-        axis: str,
-        name: str = "",
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Rectangle
-
-        Parameters
-        ----------
-        corner :
-            One corner of the rectangle.
-        dimensions :
-            Dimensions of the rectangle e.g., for a 2D rectangle it is a list of
-            values of width and height.
-        height : float
-            height of the rectangle
-        axis : str
-            axis perpendicular to the rectangle preceded by '+' if the panel
-            front faces the positive axis and '-' if it faces the negative
-            axis e.g., '+x', '+0', '-y' etc.
-        name : optional
-            name of the panel.
-        """
-        super().__init__(
-            simulation=simulation, shape=_smoldyn.PanelShape.rect, name=name
-        )
-        self.corner = corner
-        self.dimensions = dimensions
-        assert axis[0] in "+-", "axis must precede by '+' or '-'"
-        assert axis[1].lower() in "012xyz"
-        self.axis = axis.lower()
-        self.axisIndex = self._axisIndex(axis[1])
-        self.toGenericPanel()
-
-    def toGenericPanel(self):
-        self.axisstr = self.axis
-        self.pts = [*self.corner, *self.dimensions]
-        return self.axisstr, self.pts
-
-
-class Triangle(Panel):
-    def __init__(
-        self,
-        *,
-        vertices: Sequence[Sequence[float]] = [[]],
-        name: str = "",
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Triangle Panel.
-
-        Parameters
-        ----------
-        vertices :
-            vertices of triangle.
-        name :
-            name
-        """
-        super().__init__(
-            simulation=simulation, shape=_smoldyn.PanelShape.tri, name=name
-        )
-        self.axisstr = ""
-        self.vertices = vertices
-        self.pts = functools.reduce(operator.iconcat, vertices, [])
-
-
-class Sphere(Panel):
-    def __init__(
-        self,
-        *,
-        center: List[float],
-        radius: float,
-        slices: int,
-        stacks: int = 0,
-        name: str = "",
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Sphere
-
-        Parameters
-        ----------
-        center :
-            The center of the sphere.
-        radius : float
-            The radius of the sphere.
-        slices: int
-            Number of slices (longitudnal lines) that are used for drawing the sphere.
-        stacks: int
-            Number of stacks (latitude lines, default 0) that are used to drawing the sphere. `
-            If a non-postive number is given,`slices` value is used.
-        name : optional
-            name of the panel. If omitted, 0, 1, 2 etc. will be assigned.
-        """
-        super().__init__(
-            simulation=simulation, shape=_smoldyn.PanelShape.sph, name=name
-        )
-        self.center = center
-        self.radius = radius
-        self.slices = slices
-        assert self.slices > 0, "Positive int is required"
-        self.stacks = stacks if stacks > 0 else slices
-        # Smoldyn panel
-        self.axisstr = ""
-        self.pts = [*self.center, self.radius, self.slices, self.stacks]
-
-
-class Hemisphere(Panel):
-    def __init__(
-        self,
-        *,
-        center: List[float],
-        radius: float,
-        vector: List[float],
-        slices: int,
-        stacks: int,
-        name: str = "",
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Hemisphere
-
-        Parameters
-        ----------
-        center :
-            The center of hemisphere
-        radius : float
-            The radius of the hemisphere. Enter a positive radius to have the
-            front of the surface on the outside and a negative radius for it to
-            be on the inside.
-        vector :
-            The outward pointing vector (needs NOT be normalized)
-        slices : int
-            The number of slices
-        stacks : int
-            The number of stacks
-        name : optional
-            name
-        """
-        super().__init__(
-            simulation=simulation, shape=_smoldyn.PanelShape.hemi, name=name
-        )
-        self.center = center
-        self.radius = radius
-        self.vector = vector
-        self.slices = slices
-        self.stacks = stacks
-        # Smoldyn Panel
-        self.axisstr = ""
-        self.pts = [*self.center, self.radius, *self.vector, self.slices, self.stacks]
-
-
-class Cylinder(Panel):
-    def __init__(
-        self,
-        *,
-        start: List[float],
-        end: List[float],
-        radius: float,
-        slices: int,
-        stacks: int,
-        name: str = "",
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Cylinder
-
-        Parameters
-        ----------
-        start :
-            Cylinder axis start point
-        end :
-            Cylinder axis's end point
-        radius : float
-            The radius of the cylinder. If the radius is negative then the front
-            of the surface is on the inside otherwise it is on the outside.
-        slices : int
-            Number of slices
-        stacks : int
-            Number of stacks
-        name : optional
-            name
-        """
-        super().__init__(
-            simulation=simulation, shape=_smoldyn.PanelShape.cyl, name=name
-        )
-        self.start: List[float] = start
-        self.end: List[float] = end
-        self.radius: float = radius
-        self.slices: int = slices
-        self.stacks: int = stacks
-        # Smoldyn panel
-        self.axisstr: str = ""
-        self.pts = [*self.start, *self.end, self.radius, self.slices, self.stacks]
-
-
-class Disk(Panel):
-    def __init__(
-        self,
-        *,
-        center: List[float],
-        radius: float,
-        slices: int,
-        vector: List[float],
-        name="",
-        simulation: Optional[_smoldyn.Simulation] = None,
-    ):
-        """Disk
-
-        Parameters
-        ----------
-        center :
-            center of the disk.
-        radius : float
-            radius of the disk.
-        slices : int
-            Number of slices for drawing.
-        vector:
-            A vector that points away from the front of the disk. The size of
-            this vector is 2 for 2-D and 3 for 3-D.
-        name: optional
-            name of this Disk.
-        """
-        super().__init__(
-            simulation=simulation, shape=_smoldyn.PanelShape.disk, name=name
-        )
-        assert slices > -1, f"Slices must be positive. Given value {slices}"
-        self.center = center
-        self.radius = radius
-        self.slices = slices
-        self.vector = vector
-        # Smoldyn panel
-        self.axisstr = ""
-        # From the manual: #Slice is entered last (after normal vector).
-        self.pts = [*self.center, self.radius, *self.vector, self.slices]
-
-
-class _PanelFace(object):
-    def __init__(self, *, simulation: _smoldyn.Simulation, name: str, panel: Panel):
-        self.simulation = simulation
-        assert name in ["front", "back"]
-        self.name = _smoldyn.PanelFace.__members__[name]
-        self.panel = panel
-
-    def jumpTo(self, toface, bidirectional: bool = False):
-        """Add a jump reaction between two panels of same Surface
-
-        See also
-        --------
-        Panel.jumpTo
-        """
-        assert (
-            self.panel.ctype == toface.panel.ctype
-        ), "Both panels must have same geometry"
-        assert (
-            self.panel.surface == toface.panel.surface
-        ), "Both panels must have same surface"
-        __logger__.debug(
-            f"{self.panel.surface.name}, {self.panel.name} "
-            f", {self.name}, {toface.panel.name}, {toface.name}, "
-            f"{bidirectional}"
-        )
-        k = self.simulation.setPanelJump(
-            self.panel.surface.name,
-            self.panel.name,
-            self.name,
-            toface.panel.name,
-            toface.name,
-            bidirectional,
-        )
-        assert k == _smoldyn.ErrorCode.ok
-
-
-class _SurfaceFaceCollection(object):
-    def __init__(
-        self, simulation: _smoldyn.Simulation, faces: List[str], surfname: str
-    ):
-        """Collection of faces of a surface"""
-        self.simulation = simulation
-        self.faces: List[str] = faces
-        self.surfname: str = surfname
-        self.__valid_actions_ = [
-            "reflect",
-            "trans",
-            "absorb",
-            "jump",
-            "port",
-            "mult",
-            "no",
-            "none",
-        ]
-
-    def setStyle(
-        self,
-        color: ColorType = "",
-        drawmode: str = "none",
-        thickness: float = 1.0,
-        stipplefactor: int = -1,
-        stipplepattern: int = -1,
-        shininess: int = -1,
-    ):
-        """Set drawing style for the face of surface.
-
-        Parameters
-        ----------
-        drawmode : str
-            May be "none", "vertex", "edge", "face", or combinations of ‘v’,
-            ‘e’, or ‘f’ for multiple renderings of vertices, edges, and/or
-            faces. 2-D spheres and hemispheres are either filled or are
-            outlined depending on the polygon frontcharacter. If multiple
-            renderings are chosen in 3D, then panel faces are shown in the
-            requested color and other renderings are shown in black.
-        thickness : float
-            Boldness of the surface in pixels for drawing purposes.  This is
-            only relevant for 1-D and 2-D simulations, and for 3-D simulations
-            in which surfaces are drawn with just vertices or edges and not
-            faces.
-        color : Color
-            color e.g. 'black', 'red', [0.1,0.1,0.1] etc.
-        stipplefactor : int
-            stipplefactor is the repeat distance for the entire stippling
-            pattern (1 is a good choice).  Stippling of the surface edges, for
-            drawing purposes.  This is only relevant for 3-D simulations in
-            which surfaces are drawn with just edges and not faces, and with
-            opengl_good or opengl_better display method.
-        stipplepattern : int
-            stipplepattern a hexidecimal integer, enter the stippling pattern between
-            ``0x0000`` (0) and ``0xFFFF`` (65536), ``0x00FF`` (256) has long dashes,
-            ``0x0F0F`` (3855) has medium dashes, ``0x5555`` (21845)  has dots, etc.
-            Turn stippling off with ``0xFFFF`` (65536).
-        shininess : float
-            Shininess of the surface for drawing purposes.  This value can
-            range from 0 for visually flat surfaces to 128 for very shiny
-            surfaces.  This is only relevant for some simulations.
-        """
-        for which in self.faces:
-            # TODO : Check on drawmode
-            k = self.simulation.setSurfaceStyle(
-                self.surfname,
-                _smoldyn.PanelFace.__members__[which],
-                _smoldyn.DrawMode.__members__[drawmode],
-                thickness,
-                Color(color).rgba,
-                stipplefactor,
-                stipplepattern,
-                shininess,
-            )
-            assert k == _smoldyn.ErrorCode.ok, f"Failed to set drawing style {k}"
-
-    def setAction(
-        self,
-        species: Union[Species, List[Species]],
-        action: str,
-        new_species: Optional[Species] = None,
-    ):
-        """The behavior of molecules named species when they collide with this
-        face of this surface.
-
-        Parameters
-        ----------
-        species :
-            List of species or a single species. DO NOT use the name of
-            species.
-        action : str
-            The action can be  `“reflect”`, `“absorb”`, `“transmit”`, `“jump”`,
-            `“port”`, or `“periodic”`.
-        new_species:
-            TODO: Implement it.
-            If `new_species` is entered, then the molecule changes to this new
-            species upon surface collision. In addition, it’s permissible to
-            enter the action as “multiple,” in which case the rates need to be
-            set with rate; alternatively, just setting the rates will
-            automatically set the action to “multiple.” The default is
-            transmission for all molecules.
-        """
-        assert (
-            action in self.__valid_actions_
-        ), f"'{action}' is not a valid action. Available actions: {', '.join(self.__valid_actions_)}"
-
-        if isinstance(species, str):
-            raise NameError(
-                "This API does not accepts species by their names or the keyword 'all'."
-                " Please pass the objects."
-            )
-        listSpecies = [species] if isinstance(species, Species) else species
-        for sp in listSpecies:
-            if isinstance(sp, Species):
-                sname, sstate = sp.name, sp.state
-            else:
-                sname, sstate = sp, _smoldyn.MolecState.soln
-
-            if isinstance(sstate, str):
-                sstate = _smoldyn.MolecState.__members__[sstate]
-
-            # TODO: see issue #17
-            if new_species:
-                raise NotImplementedError("This feature is not implemented.")
-
-            for which in self.faces:
-                k = self.simulation.setSurfaceAction(
-                    self.surfname,
-                    _smoldyn.PanelFace.__members__[which],
-                    sname,
-                    sstate,
-                    _smoldyn.SrfAction.__members__[action],
-                )
-                assert k == _smoldyn.ErrorCode.ok, f"Failed setSurfaceAction: {k}"
-
-
-class Path2D(object):
-    def __init__(self, *points, simulation: _smoldyn.Simulation, closed: bool = False):
-        """Construct a 2D path from given points.
-
-        A Path2D consists of `Rectangle` and `Triangle`.
-
-        Parameters
-        ----------
-        *points:
-            Points
-        simulation:
-            _smoldyn.Simulation object.
-        closed: bool
-            If closed is `True`, the last point and the first point are
-            connected. Default `False`.
-        """
-        self.points = list(points)
-
-        self.simulation = simulation
-        assert self.simulation
-
-        if closed and self.points[0] != self.points[-1]:
-            self.points.append(self.points[0])
-        self.panels: List[Panel] = []
-        for p1, p2 in zip(self.points, self.points[1:]):
-            (x1, y1), (x2, y2) = p1, p2
-            theta = math.atan2(y2 - y1, x2 - x1)
-            __logger__.debug(f"theta={theta} {p1} and {p2}")
-            if theta in [0.0, math.pi, math.pi / 2.0, -math.pi / 2.0]:
-                if theta == 0.0:
-                    axis = "+y"
-                elif theta == math.pi:
-                    axis = "-y"
-                elif theta == math.pi / 2.0:
-                    axis = "-x"
-                elif theta == -math.pi / 2.0:
-                    axis = "+x"
-                else:
-                    raise RuntimeError(
-                        "Should not be here."
-                        " Python3 numerical computation is broken!"
-                    )
-                length = x2 - x1 if y2 == y1 else y2 - y1
-                p = Rectangle(
-                    simulation=self.simulation,
-                    corner=(x1, y1),
-                    dimensions=[length],
-                    axis=axis,
-                )
-                __logger__.info(f"Added a Rectangle {p}")
-                self.panels.append(p)
-            else:
-                t = Triangle(simulation=self.simulation, vertices=((x1, y1), (x2, y2)))
-                self.panels.append(t)
-
-
-# TODO: Add a Path3D or Surface3D. not sure what to call it.
-
-
-class Surface(object):
-    """Surfaces are infinitesimally thin structures that can be used to
-    represent cell membranes, obstructions, system boundaries, or other things.
-
-    Note
-    ----
-
-    They are 2D structures in 3D simulations, or 1D lines or curves in 2D simulations (or 0D points
-    in 1D simulations).Each surface has a “front” and a “back” face, so molecules can interact
-    differently with the two sides of a surface.Each surface is composed of one or more
-    “:py:class:`~Panels`”, where each panels can be a rectangle, triangle, sphere, hemisphere,
-    cylinder, or a disk. Surfaces can be disjoint, with separate non-connected portions.  However,
-    all portions of a given surface type are displayed in the same way and interact with molecules
-    in the same way.
-
-    """
-
-    def __init__(
-        self, *, simulation: _smoldyn.Simulation, name: str, panels: List[Panel]
-    ):
-        """
-        Parameters
-        ----------
-        simulation:
-            Simulation object
-        panels : List[Panel]
-            List of panels. A surface must have at least one.
-        name : str
-            name of the surface
-
-        Examples
-        --------
-        >>> r1 = S.Rectangle(corner=[100,0,0], dimensions=[100,100], axis='-x')
-        >>> r2 = S.Rectangle(corner=[0,0,0], dimensions=[100,100], axis='+y')
-        >>> s = smoldyn.Surface("walls", panels=["r1", "r2"])
-        """
-        self.simulation = simulation
-        assert self.simulation
-
-        self.panels = panels
-        self.name = name
-        self.simulation.addSurface(self.name)
-
-        self.front = _SurfaceFaceCollection(self.simulation, ["front"], name)
-        self.back = _SurfaceFaceCollection(self.simulation, ["back"], name)
-        self.both = _SurfaceFaceCollection(self.simulation, ["front", "back"], name)
-        self._addPanelsToSmoldyn()
-
-    def _addPanelsToSmoldyn(self):
-        """Call libsmodyn API to construct this surface' Panels"""
-        assert self.name, "Surface name is missing"
-        for i, panel in enumerate(self.panels):
-            panel.name = panel._getName(i)
-            panel.surface = self
-
-            # Set simulation object before adding Panel.
-            panel._setSimulation(self.simulation)
-
-            # Add panels.
-            k = self.simulation.addPanel(
-                self.name,
-                panel.ctype,
-                panel.name,
-                panel.axisstr,
-                panel.pts,
-            )
-            assert (
-                k == _smoldyn.ErrorCode.ok
-            ), f"Failed to add panel (error={k}): Surface:{self.name} {panel}"
-
-    def setStyle(self, face, *args, **kwargs):
-        """See the function :func:`_SurfaceFaceCollection.setStyle` for more
-        details. This function forwards arguments to
-        :func:`_SurfaceFaceCollection.setStyle`.
-
-        Parameters
-        ----------
-        face: str
-            face of the surface: 'front', 'back', 'both'
-        *args:
-            See :func:`_SurfaceFaceCollection.setStyle`
-        **kwargs:
-            See :func:`_SurfaceFaceCollection.setStyle`
-
-        See Also
-        --------
-        :func:`_SurfaceFaceCollection.setStyle`
-        """
-        assert face in ["front", "back", "both"]
-        getattr(self, face).setStyle(*args, **kwargs)
-
-    def setAction(
-        self,
-        face: str,
-        species: Union[Species, List[Species]],
-        action: str,
-        new_species: Optional[Species] = None,
-    ):
-        """Set drawing style for the face of surface
-        (calls :func:`_SurfaceFaceCollection.setAction`)
-
-        Parameters
-        ----------
-        face: str
-            face of the surface: 'front', 'back', 'both'
-        species :
-            List of species or a single species. DO NOT use the name of
-            species.
-        action : str
-            The action can be  `“reflect”`, `“absorb”`, `“transmit”`, `“jump”`,
-            `“port”`, or `“periodic”`.
-        new_species:
-            TODO: Implement it.
-            If `new_species` is entered, then the molecule changes to this new
-            species upon surface collision. In addition, it’s permissible to
-            enter the action as “multiple,” in which case the rates need to be
-            set with rate; alternatively, just setting the rates will
-            automatically set the action to “multiple.” The default is
-            transmission for all molecules.
-
-
-        See Also
-        --------
-        :func:`_SurfaceFaceCollection.setAction`
-        """
-        getattr(self, face).setAction(species, action, new_species)
-
-    def addMolecules(
-        self,
-        species: SpeciesWithState,
-        N: int,
-        panels: Optional[List[Panel]] = None,
-        pos: List[float] = [],
-    ):
-        """Place molecules with random or specific positions onto a given
-        surface (optionally specified panels).
-
-        Parameters
-        ----------
-        species:
-            Species to add, a Species or a tuple of (Species, MolecState)
-            e.g. (A, 'front')
-        N : int
-            number of molecules
-        surface : smoldyn.geometry.Surface
-            Surface
-        panels: smoldyn.geometry.Panel
-            Panels of surface. If `None` is given then all panels of
-            surfece are used.
-        pos: List[float]
-            Position of the molecules. If not given, then randomly distribute
-            the molecules onto the surface/panels.
-        """
-        assert N > 0, "Expected a positive number"
-        assert species
-        if isinstance(species, Species):
-            sname = species.name
-            sstate = species.state
-        else:
-            assert len(species) == 2, "Expected tuple of (Species, MolecState)"
-            sname = species[0].name
-            sstate = _toMS(species[1])
-
-        panels = panels if panels is not None else self.panels
-
-        # Distribute molecules equally among the panels.
-        _N = N // len(panels)
-        Ns = [_N] * len(panels)
-        Ns[0] += N - sum(Ns)
-        assert sum(Ns) == N
-
-        for panel, _n in zip(panels, Ns):
-            assert panel
-            assert panel.ctype
-            k = self.simulation.addSurfaceMolecules(
-                sname,
-                sstate,
-                _n,
-                self.name,
-                panel.ctype,
-                panel.name,
-                pos,
-            )
-            assert k == _smoldyn.ErrorCode.ok, k
-
-    def _setRate(
-        self,
-        species: SpeciesWithState,
-        state1: SpeciesState,
-        state2: SpeciesState,
-        rate: float,
-        new_species: Optional[Species] = None,
-        isinternal: bool = False,
-    ):
-        if not isinstance(species, Species):
-            sname, sstate = species[0].name, species[1]
-        else:
-            sname, sstate = species.name, species.state
-        state1 = _toMS(state1)
-        new_species_str = new_species.name if new_species else ""
-        k = self.simulation.setSurfaceRate(
-            self.name,
-            sname,
-            _toMS(sstate),
-            _toMS(state1),
-            _toMS(state2),
-            rate,
-            new_species_str,
-            isinternal,
-        )
-        assert k == _smoldyn.ErrorCode.ok, "Failed to set rate"
-
-    def setRate(
-        self,
-        species: SpeciesWithState,
-        state1: SpeciesState,
-        state2: SpeciesState,
-        rate: float,
-        revrate: float = 0.0,
-        new_species: Optional[Species] = None,
-        isinternal: bool = False,
-    ):
-        """The rate constant for transitions from `state1` to `state2` of molecules
-        named `species`.
-
-        Parameters
-        ----------
-        species : SpeciesWithState
-            A species or a tuple of `Species` and its state.
-        state1 : SpeciesState
-            Can be any of: fsoln, bsoln (in solution, hitting the front or
-            back of the panel, respectively), front, back, up, or down.
-        state2 : SpeciesState
-            Can be any of: fsoln, bsoln (in solution, hitting the front or
-            back of the panel, respectively), front, back, up, or down.
-        rate : float
-            rate (must be on-zero positive value).
-        revrate: float
-            reverse rate (default 0.0). If this value is a positive non-zero
-            value, then a reverse rate is also set.
-        new_species :
-            newspecies
-        isinternal:
-            When set to `True`, a different value is entered. Instead of
-            entering the surface action rate, enter the probability of the
-            action at each collision.  Probabilities for reflection are ignored
-            since they are calculated as the probability that the molecule does
-            not transmit, absorb, or jump.
-        """
-        self._setRate(species, state1, state2, rate, new_species, isinternal)
-        if revrate > 0.0:
-            self._setRate(species, state2, state1, revrate, new_species, isinternal)
-
-
-class NullSurface(Surface):
-    def __init__(self):
-        self.name = ""
-        self.panels = []
-
-    def __bool__(self):
-        return False
-
-
-class Port(object):
-    """Ports are data structures that are used for importing and
-    exporting molecules between a Smoldyn simulation and another simulation.  In
-    particular, they are designed for the incorporation of Smoldyn into MOOSE,
-    but they could also be used to connect multiple Smoldyn simulations or for
-    other connections.
-
-    A port is essentially a surface and a buffer. Smoldyn
-    molecules that hit the porting surface are removed from the Smoldyn
-    simulation and are put into the buffer for export.  Once exported, they are
-    removed from the buffer.  Also, molecules may be added to the Smoldyn
-    simulation at the porting surface by other programs.
-    """
-
-    def __init__(
-        self,
-        simulation: _smoldyn.Simulation,
-        *,
-        name: str,
-        surface: Union[Surface, str],
-        panel: str,
-    ):
-        """
-        Parameters
-        ----------
-        simulation:
-            _smoldyn.Simulation() object
-        name : str
-            name of the port
-        surface : Union[Surface,str]
-            Porting surface (must be created before).
-        panel : str
-            Face of the which surface active for porting: "front" or "back".
-        """
-        self.simulation = simulation
-        self.name: str = name
-        self.surfname = surface.name if isinstance(surface, Surface) else surface
-        assert panel in ["front", "back"]
-        self.panel = _smoldyn.PanelFace.__members__[panel]
-        k = self.simulation.addPort(self.name, self.surfname, self.panel)
-        assert k == _smoldyn.ErrorCode.ok
-
-
-class Compartment(object):
-    def __init__(
-        self,
-        simulation: _smoldyn.Simulation,
-        name: str,
-        *,
-        surface: Union[str, Surface],
-        point: List[float],
-    ):
-        """Comapartment.
-
-        Parameters
-        ----------
-        name : str
-            name of the compartment.
-        surface : Union[str, Surface]
-            Name of the bounding surface for this compartment.
-        point : List[float]
-            An interior-defining point for this compartment.
-        """
-        self.name = name
-        self.srfname = surface.name if isinstance(surface, Surface) else surface
-        self.point = point
-        self.simulation = simulation
-        assert self.point, "At least one point is required."
-        k = self.simulation.addCompartment(self.name)
-        assert k == _smoldyn.ErrorCode.ok
-        k = self.simulation.addCompartmentSurface(self.name, self.srfname)
-        assert k == _smoldyn.ErrorCode.ok
-        k = self.simulation.addCompartmentPoint(self.name, self.point)
-        assert k == _smoldyn.ErrorCode.ok
-
-    def addMolecules(self, species: Species, N: int):
-        """Place number of molecules in a compartment (uniformly distributed).
-
-        Parameters
-        ----------
-        N : int
-            number of molecules
-        species : Species
-            Species to add
-
-        See also
-        --------
-        :py:class:`smoldyn.kinetics.Species.addToCompartment`
-        """
-        assert N > 0, "Needs a positive number"
-        k = self.simulation.addCompartmentMolecules(species.name, N, self.name)
-        assert k == _smoldyn.ErrorCode.ok
-
-
-class Reaction(object):
-    __methoddict__ = dict(
-        i="irrev",
-        p="pgem",
-        x="pgemmax",
-        y="pgemmax2",
-        r="ratio",
-        b="unbindrad",
-        q="pgem2",
-        s="ratio2",
-        o="offset",
-        f="fixed",
-    )
-
-    def __init__(
-        self,
-        simulation: _smoldyn.Simulation,
-        name: str,
-        subs: List[SpeciesWithState],
-        prds: List[SpeciesWithState],
-        *,
-        rate: float = 0.0,
-        compartment: Compartment = None,
-        surface: Surface = None,
-        binding_radius: float = 0.0,
-        reaction_probability: float = 0.0,
-    ):
-        """Reaction (only occurs in forwared direction).
-
-        Parameters
-        ----------
-        simulation: _smoldyn.Simulation
-            Simulation object
-        name: str
-            name of the reaction.
-        subs : List[SpeciesWithState]
-            List of rectants.
-        prds : List[SpeciesWithState]
-            List of products.
-        rate : float
-            rate of the reaction
-        compartment: Compartment
-            If not ``None``, restrict the reaction to this compartment.
-        surface: Surface
-            If not ``None``, restricts this reaction to this surface.
-        binding_radius: float
-            binding radius (for second order reactions, if kf is not given)
-        reaction_probability: float
-            reaction probability (for first order reactions, if kf if not
-            given)
-        """
-        self.simulation = simulation
-        self.name = "r%d" % id(self) if not name else name
-        self.__rate = 0.0
-        self.subs = subs
-        self.prds = prds
-        self.reaction_probability = reaction_probability
-        self.binding_radius = binding_radius
-        self.compartment = compartment
-        self.surface = surface
-
-        assert len(subs) < 3, "At most two reactants are supported."
-        if subs is None or len(subs) == 0:
-            assert len(prds) > 0, "At least one product for a zero-order reaction."
-            subs = [NullSpecies()]
-        r1 = subs[0]
-        r2 = subs[1] if len(subs) == 2 else NullSpecies()
-
-        if isinstance(r1, Species):
-            r1name, r1state = r1.name, _toMS(r1.state)
-        else:
-            assert len(r1) == 2, "Expected tuple of (Species, state) e.g. (A, 'front')"
-            r1name = r1[0].name
-            r1state = _toMS(r1[1])
-
-        if isinstance(r2, Species):
-            r2name, r2state = r2.name, _toMS(r2.state)
-        else:
-            assert len(r2) == 2, "Expected tuple of (Species,state) e.g. (S, 'back')"
-            r2name, r2state = r2[0].name, _toMS(r2[1])
-
-        prdNames, prdStates = [], []
-        for x in prds:
-            if isinstance(x, Species):
-                prdNames.append(x.name)
-                prdStates.append(_toMS(x.state))
-            else:
-                prdNames.append(x[0].name)
-                prdStates.append(_toMS(x[1]))
-
-        k = self.simulation.addReaction(
-            name,
-            r1name,
-            r1state,
-            r2name,
-            r2state,
-            prdNames,
-            prdStates,
-            rate,
-        )
-        if k != _smoldyn.ErrorCode.ok:
-            __logger__.warning(f" Substrates: {subs}")
-            __logger__.warning(f" Products: {prds}, {prdNames}/{prdStates}")
-            raise RuntimeError(f"Failed to add reaction, ErrorCode {k}")
-
-        self.setRate(rate, reaction_probability, binding_radius)
-        if self.compartment is not None or self.surface is not None:
-            cname = self.compartment.name if self.compartment else ""
-            sname = self.surface.name if self.surface else ""
-            assert cname or sname
-            k = self.simulation.setReactionRegion(self.name, cname, sname)
-            assert k == _smoldyn.ErrorCode.ok
-
-    @property
-    def rate(self):
-        return self.__rate
-
-    @rate.setter
-    def rate(self, rate: float):
-        if rate != self.__rate:
-            self.__rate = rate
-            self.setRate(rate)
-
-    def setRate(self, rate, reaction_probability=-1.0, binding_radius=-1.0):
-        # if rate is negative, then we expect either binding_radius or
-        # reaction_probability. A reaction can have zero rate.
-        if rate >= 0.0:
-            k = self.simulation.setReactionRate(self.name, rate, False)
-            assert k == _smoldyn.ErrorCode.ok
-            return
-        elif rate < 0.0:
-            # check if reaction_probability is given
-            if len(self.subs) < 2:
-                assert (
-                    reaction_probability >= 0.0
-                ), "Must set rate or reaction_probability"
-                k = self.simulation.setReactionRate(
-                    self.name, reaction_probability, True
-                )
-                assert k == _smoldyn.ErrorCode.ok
-            else:
-                if reaction_probability >= 0.0:
-                    k = self.simulation.setReactionRate(self.name, reaction_probability, 2)
-                    assert k == _smoldyn.ErrorCode.ok
-                if binding_radius >= 0.0:
-                    k = self.simulation.setReactionRate(self.name, binding_radius, True)
-                    assert k == _smoldyn.ErrorCode.ok
-        else:
-            raise RuntimeError(
-                "Rate is not a numeric value"
-            )
-
-    @property
-    def order(self):
-        return len(self.subs)
-
-    def setIntersurface(self, rules: List[Union[int, str]]):
-        """Define `rules` to allow a bimolecular reaction operates when its
-        reactants are on different surfaces. In general, there should be as
-        many rule values as there are products for this reaction
-
-        Parameters
-        ----------
-        rules :
-            List of integer or string. For each product choose `1` (or
-            ``"r1"``) if it should be placed on the first reactant’s surface or
-            relative to that surface, and `2` (``"r2"``) if it should be placed
-            on the second reactant’s surface or relative to that surface. To
-            turn off intersurface reactions, which is the default behavior,
-            give rule_list as ``[-1]`` or ``None``.  To turn on intersurface
-            reactions for reactions that have no products, give rule_list as
-            ``[0]`` or ``[]``. This statement cannot be used together with the
-            ``setSerialNum`` function for the same reaction.
-
-        """
-        assert self.order == 2, "Bimoleculear reaction is needed."
-        assert len(rules) == len(
-            self.prds
-        ), "Length of rules should be equal to number of products"
-        rules = [-1] if rules is None else rules
-        rules = [0] if rules == [] else rules
-        _rules: List[int] = []
-
-        # r1, r2 are turned to 1, 2 etc.
-        for r in rules:
-            r = int(r[1:]) if isinstance(r, str) else int(r)
-            _rules.append(r)
-        k = self.simulation.setReactionIntersurface(self.name, _rules)
-        assert k == _smoldyn.ErrorCode.ok
-
-    def productPlacement(
-        self,
-        method: str,
-        param: float = 0.0,
-        product: str = "",
-        pos: List[float] = [],
-    ):
-        """Placement method and parameters for the products of reaction.
-        This also affects the binding radius of the reverse reaction, as
-        explained in the manual.
-
-        Parameters
-        ----------
-        method : 'irrev' ('i'), 'pgem' ('p'), 'pgemmax' ('x')
-            , 'pgemmax2' ('y'), 'ratio' ('r'), 'unbindrad' ('b')
-            , 'pgem2' ('q'), 'ratio2' ('s'), 'offset' ('o'), 'fixed' ('f')
-        param : float
-            Parameter value. Usually required except for type 'irrev'
-        product: str, optional
-            Required for type 'fixed' and 'offset'
-        pos:
-            Required for type 'fixed' and 'offset'
-
-        Notes
-        -----
-        To create a “bounce” type reaction, for simulating excluded volume,
-        enter the type as bounce.  In this case, enterno parameter for the
-        default algorithm orone parameter.The default algorithm, also entered
-        with a -2 parameter, performs ballistic reflection for spherical
-        molecules. Enter a parameter of -1 for an algorithm in which the reactant
-        edges get separated by the same amount as they used to overlap, along
-        their separation vector (e.g. consider two reactants each of radius 1,
-        so the binding radius is set to 2; then, if the center-to-center
-        distance is found to be 1.6, the molecules get separated to make the
-        center-to-center distance equal to 2.4).  Alternatively, you can use
-        the parameter value to define the new separation, which should be
-        larger than the binding radius.
-        """
-        method = self.__methoddict__.get(method, method)
-        revType = _smoldyn.RevParam.__members__[method]
-
-        if method in ["fixed", "offset"]:
-            assert product, "Product is required"
-            assert pos, "pos is required"
-        k = self.simulation.setReactionProducts(self.name, revType, param, product, pos)
-        assert k == _smoldyn.ErrorCode.ok
-
-
-class BidirectionalReaction(object):
-    def __init__(
-        self,
-        simulation: _smoldyn.Simulation,
-        name: str,
-        subs: List[SpeciesWithState],
-        prds: List[SpeciesWithState],
-        kf: float,
-        kb: float = 0.0,
-        *,
-        binding_radius: float = 0.0,
-        reaction_probability: float = 0.0,
-        compartment: Compartment = None,
-        surface: Surface = None,
-    ):
-        """A bidirectional chemical reaction that consists of two Reactions,
-        forward  (always present) and reverse (`None` if ``kb<=0.0``).
-
-        Parameters
-        ----------
-        simulation: _smoldyn.Simulation
-            Simulation object
-        name : str
-            name of the reaction.
-        subs : List[SpeciesWithState]
-            subtrates
-        prds : List[SpeciesWithState]
-            products
-        kf : float
-            Forward rate constant
-        kb : float
-            Backward rate constant (default 0.0)
-        binding_radius: float
-            Binding radius (for second order reaction)
-        reaction_probability: float
-            Reaction probability (first order reaction)
-        compartment : Compartment
-            Reaction compartment. If not `None`, both forward and reverse
-            reactions will be limited to this compartment.
-        surface : Surface
-            Reaction surface. If not `None`, both forward and reverse
-            reactions will be limited to this surface.
-        """
-        self.simulation = simulation
-        self.name = f"r{id(self):d}" if not name else name
-        fwdname, revname = (name + "fwd", name + "rev") if kb > 0.0 else (name, "")
-        self._kf = kf
-        self._kb = kb
-        self.forward = Reaction(
-            self.simulation,
-            fwdname,
-            subs,
-            prds,
-            rate=kf,
-            compartment=compartment,
-            surface=surface,
-            binding_radius=binding_radius,
-            reaction_probability=reaction_probability,
-        )
-
-        self.reverse = None
-        if self._kb > 0.0:
-            self.reverse = Reaction(
-                self.simulation,
-                revname,
-                prds,
-                subs,
-                rate=self._kb,
-                compartment=compartment,
-                surface=surface,
-            )
-
-    @property
-    def kf(self):
-        return self._kf
-
-    @kf.setter
-    def kf(self, val: float):
-        self.forward.setRate(val)
-
-    @property
-    def kb(self):
-        return self._kh
-
-    @kb.setter
-    def kb(self, val: float):
-        assert self.reverse
-        self.reverse.setRate(val)
-
-
-@dataclass
-class Partition(object):
-    simulation: _smoldyn.Simulation
-    name: str
-    value: float
-
-    def __post_init__(self):
-        """Sets the virtual partitions in the simulation volumne. Two
-        specialization is avaiable: :py:class:`MoleculePerBox`, and
-        :py:class:`Box`.
-
-        See also
-        --------
-        :py:class:`MoleculePerBox`
-        :py:class:`Box`
-        """
-        k = self.simulation.setPartitions(self.name, self.value)
-        assert k == _smoldyn.ErrorCode.ok, f"Failed to set partition: {k}"
-
-
-class MoleculePerBox(Partition):
-    def __init__(self, simulation: _smoldyn.Simulation, size: float):
-        warnings.warn(
-            "MoleculePerBox is deprecated. Please use setPartitions in the future",
-            DeprecationWarning,
-        )
-        super().__init__(simulation, "molperbox", size)
-
-
-class Box(Partition):
-    def __init__(self, simulation: _smoldyn.Simulation, size):
-        warnings.warn(
-            "Box is deprecated. Please use setPartitions in the future",
-            DeprecationWarning,
-        )
-        super().__init__(simulation, "boxsize", size)
-
-
-def addMoleculesToSolution(molecule, *args, **kwargs):
-    """Add molecules to the solution.
-
-    An alias of Species.addToSolution
-
-    See also
-    --------
-    Species.addToSolution
-    """
-    molecule.addMoleculesToSolution(*args, **kwargs)
-
-
-class Simulation(_smoldyn.Simulation):
-    """Simulation class. A :class:`Simulation` object is an unit of simulation.
-    it is recommended to create a :class:`Simulation` object for every standalone
-    model.
-
-    Note
-    ----
-
-    Every model starts with a Simulation object which has its unique
-    :class:`simstruct`. Note that a user can create as many arbitrary smoldyn
-    objects as one likes but these objects become active only when they
-    are added to a :class:`Simulation` object.
-
-    See also
-    --------
-
-    :class:`_smoldyn.Simulation`
-
-    """
-
-    def __init__(
-        self,
-        low: List[float],
-        high: List[float],
-        *,
-        boundary_type: BoundType = "r",
-        log_level: int = 3,
-        **kwargs,
-    ):
-        """Simulation class is a container for a complete model. An object of
-        this class is a stand-alone self-contained model.
-
-        Parameters
-        ----------
-        low:
-            Lower bound.
-        high:
-            Higher bound.
-
-        log_level: int, default 3
-            set log level for default logger.
-            1: DEBUG, 2: INFO, 3: WARNING, 4: ERROR, 5: CRITICAL
-
-        Other Parameters
-        ----------------
-        stop: `float`
-            Simulation stop time
-        dt: `float`
-            Simulation dt
-        start : `float`
-            Simulation start time.
-        output_files :
-            Declare output files that can be used in addCommand string.
-        seed: `int`
-            Set the random seed for the simulation.
-
-        See also
-        --------
-        :py:_smoldyn.simptr
-        """
-
-        # https://stackoverflow.com/a/50886750/1805129
-        logging.getLogger(__name__).setLevel(10 * log_level)
-        for handler in __logger__.handlers:
-            handler.setLevel(10 * log_level)
-
-        __logger__.info(f"Setting logging level to {log_level}")
-
-        assert low, f"You must pass low bound, current value {low}"
-        assert high, f"You must pass high bound, current value {high}"
-        if isinstance(boundary_type, str):
-            if len(boundary_type) == 1:
-                assert len(low) == len(
-                    high
-                ), f"dimension mismatch {len(low)} != {len(high)}"
-                boundary_type = boundary_type * len(low)
-            boundary_type = list(boundary_type)
-
-        super().__init__(low, high, boundary_type)
-
-        assert self.simptr, "Fatal error: Could not create simstruct"
-
-        # set filepath and filename at simptr
-        if __top_model_file__:
-            __top_model_file__.resolve()
-            super().setModelpath(str(__top_model_file__))
-
-        assert self.simptr, "Configuration is not initialized"
-        if kwargs.get("accuracy", 0.0):
-            self.accuracy: float = kwargs["accuracy"]
-
-        self.setOutputFiles(kwargs.get("output_files", []))
-
-        if kwargs.get("seed", -1) >= 0:
-            self.randomSeed = int(kwargs["seed"])
-
-#        if kwargs.get("log_level", 2):#????
-#            self.flags = kwargs["log_level"]	# Doesn't work
-
-    @classmethod
-    def fromFile(cls, path: Union[Path, str], arg: str = ""):
-        """Create `_smoldyn.Simulation` object from model file.
-
-        Parameters
-        ----------
-        path : T.Union[Path, str]
-            path
-        arg : str
-            arg
-        """
-        #  return _smoldyn.Simulation(str(path), arg)
-        obj = cls.__new__(cls)
-        path = Path(path).resolve()  # critical.
-        super(Simulation, obj).__init__(str(path), arg)
-        return obj
-
-    def setOutputFiles(self, outfiles: List[str], append=True):
-        """Declaration of filenames that can be used for output of simulation
-        results.  Spaces are not permitted in these names.  Any previous files
-        with the same name will be overwritten.
-
-        Parameters
-        ----------
-        outfiles : List[str]
-            Output files.  If all files don't have the same parent directory,
-            last file's parent directory is used.
-        append : bool
-            If `True`, append the data to the exsiting file. Default `False`.
-
-        See also
-        --------
-        setOutputFile
-        """
-        assert isinstance(outfiles, (list, tuple)), "Expecting a list of files"
-        for outfile in outfiles:
-            self.setOutputFile(outfile, append)
-
-    def setOutputFile(self, outfile, append: bool = False):
-        """Declaration of filenames that can be used for output of simulation
-        results.  Spaces are not permitted in these names.  Any previous files
-        with the same name will be overwritten.
-
-        Parameters
-        ----------
-        outfile : Union[str, Path]
-            Output file.
-        append : bool
-            If `True`, append the data to the exsiting file. Default `False`.
-
-        See also
-        --------
-        setOutputFiles
-        """
-        outfile = Path(outfile).resolve()
-        if outfile.parent != Path("."):
-            super().setOutputPath(str(outfile.parent) + "/")
-        # FIXME: Not sure what to do with second arg here.
-        super().addOutputFile(outfile.name, 0, append)
-
-    def setGraphics(
-        self,
-        method: str,
-        iter: int = 20,
-        delay: int = 0,
-        bg_color: ColorType = "white",
-        frame_thickness: int = 2,
-        frame_color: ColorType = "black",
-        grid_thickness: int = 0,
-        grid_color: ColorType = "white",
-        text_display: Union[List, str] = "",
-    ):
-        """Set graphics parameters for this simulation.
-
-        Parameters
-        ----------
-        method : str
-            Avaibale options: "none", "opengl", "opengl_good", "opengl_better"
-        iter : int
-            Update graphics after every nth step (default 20)
-        delay : int
-            Additional delay between rendering
-        bg_color: Color
-            Background color
-        frame_thickness: int
-            Thickness of the frame that is drawn around the simulation volume,
-            in pts. Default value is 2.
-        frame_color: Color
-            Specify the color of the frame. Default value is 'black'
-        grid_thickness: int
-            Thickness of the grid lines that can be drawn to show the virtual
-            boxes. Default value is 0, so that thegrid is not drawn.
-        grid_color: Color
-            Color of the grid. Default "white" or [1,1,1,1]
-        text_display:
-            List of variables to be displayed. Or a text string containing
-            variable names e.g. 'time E S ES(front)'
-        """
-        k = super().setGraphicsParams(method, iter, delay)
-        assert k == _smoldyn.ErrorCode.ok
-        k = super().setBackgroundStyle(Color(bg_color).rgba)
-        assert k == _smoldyn.ErrorCode.ok
-        k = super().setFrameStyle(frame_thickness, Color(frame_color).rgba)
-        assert k == _smoldyn.ErrorCode.ok
-
-        if grid_thickness > 0 and grid_color != bg_color:
-            k = super().setGridStyle(grid_thickness, Color(grid_color).rgba)
-            assert k == _smoldyn.ErrorCode.ok
-
-        self.setText(text_display)
-
-    # alias for setGraphics
-    addGraphics = setGraphics
-
-    @classmethod
-    def __todisp_text__(self, x):
-        if isinstance(x, str):
-            return x
-        if isinstance(x, tuple):
-            return f"{x[0].name}({x[1]})"
-        return x.__to_disp__()
-
-    def setText(self, text_display, color: ColorType = "black"):
-        if isinstance(text_display, str):
-            text_display = text_display.strip().split(" ")
-        for item in text_display:
-            if not item:
-                continue
-            k = super().addTextDisplay(self.__todisp_text__(item))
-            assert k == _smoldyn.ErrorCode.ok, f"Failed to set '{item}'"
-
-        k = super().setTextStyle(Color(color).rgba)
-        assert k == _smoldyn.ErrorCode.ok, "Failed to set text color"
-
-    def setTiff(
-        self,
-        tiffname: str = "OpenGL",
-        minsuffix: int = 1,
-        maxsuffix: int = 999,
-        every: int = 5,
-    ):
-        """TIFF related parameters.
-
-        Parameters
-        ----------
-        tiffname : str
-            Root filename for TIFF files, which may include path information if
-            desired. Default is “OpenGL”, which leads to the first TIFF being saved as
-            “OpenGL001.tif”.
-        minsuffix : int
-            Initial suffix number of TIFF files that are saved.  Default value
-            is 1.
-        maxsuffix : int
-            Largest possible suffix number of TIFF files that are saved.  Once
-            this value has been reached, additional TIFFs cannot be saved.
-            Default value is 999.
-        every: int
-            ``every`` is the number of simulation timesteps that should elapse
-            between subsequent snapshots.
-        """
-        k = super().setTiffParams(every, str(tiffname), minsuffix, maxsuffix)
-        assert k == _smoldyn.ErrorCode.ok
-
-    def setLight(
-        self,
-        index: int,
-        ambient: Color,
-        diffuse: Color,
-        specular: Color,
-        pos: List[float],
-    ):
-        """Set the parameters for a light source, for use with opengl_better
-        quality graphics. Parameters “ambient”, “diffuse”, “specular” are for
-        the light’s colors, which are then specified with either a word or in
-        the values as red, green, blue, and optionally alpha.
-
-        Parameters
-        ----------
-        index : int
-            The light index should be between 0 and 7.
-        ambient : Color
-            ambient
-        diffuse : Color
-            diffuse
-        specular : Color
-            specular
-        pos : List[float]
-            Light’s 3-dimensional position, which is specified as x, y,and zin
-            the values. Lights specified this way are automatically enabled
-            (turned on).
-        """
-        ambient = Color(ambient).rgba
-        diffuse = Color(diffuse).rgba
-        specular = Color(specular).rgba
-        k = super().setLightParams(index, ambient, diffuse, specular, pos)
-        assert k == _smoldyn.ErrorCode.ok
-
-    def run(
-        self,
-        stop: float,
-        dt: float,
-        *,
-        start: float = 0.0,
-        display: bool = True,
-        overwrite: bool = False,
-        accuracy=None,
-        log_level: int = 3,
-        quit_at_end: bool = False,
-    ):
-        """run the simulation.
-
-        Parameters
-        ----------
-        stop :
-            stop time
-        dt :
-            dt
-        start :
-            start (default 0.0)
-        accuracy :
-            accuracy
-        overwrite:
-            Overwrite existing data files.
-        display:
-            Show graphics (default True)
-        quit_at_end:
-            When set to `True`, smoldyn won't ask for Shift+Q at the end of simulation
-            to close the OpenGL window. Same effect can be achieved by setting
-            the environment variable SMOLDYN_NO_PROMPT. It is useful for
-            running tests in batch mode.
-        """
-
-        self.stop = float(stop)
-        self.dt = float(dt)
-        self.start = float(start)
-        if accuracy is not None:
-            self.accuracy = float(accuracy)
-
-        super().setSimTimes(self.start, self.stop, self.dt)
-
-        self.quitatend = quit_at_end
-
-        assert self.dt > 0.0, f"dt can't be <= 0.0! dt={self.dt}"
-        assert self.stop > 0.0, f"stop time can't be <= 0.0! stop={self.stop}"
-
-        k = super().runSim(self.stop, self.dt, display, overwrite)
-        assert _smoldyn.ErrorCode.ok == k, f"Expected ErrorCode.ok, got {k}"
-
-    def runUntil(self, stop, dt, display: bool = True, overwrite: bool = False):
-        """Run simulation until a given time.
-
-        Parameters
-        ----------
-        stop :
-            stop
-        dt :
-            dt
-
-        display : bool
-            Enable gui display (default `True`)?
-
-        overwrite : bool
-            Overwrite existing data (default `False`)?
-        """
-        self.stop = stop
-        self.dt = float(dt)
-
-        assert self.dt > 0.0, f"dt can't be <= 0.0! dt={self.dt}"
-        assert self.stop > 0.0, f"stop time can't be <= 0.0! stop={self.stop}"
-        super().runUntil(self.stop, self.dt, display, overwrite)
-
-    def updateSim(self):
-        """updateSim"""
-        super().updateSim()
-
-    def display(self):
-        k = super().displaySim()
-        assert k == _smoldyn.ErrorCode.ok
-
-    def addCommand(self, cmd: str, cmd_type: str, **kwargs):
-        """Add command.
-
-        Parameters
-        ----------
-        cmd: str
-            Command string.
-
-        cmd_type: str
-            Type of command. Optional when `from_string` is set to `True`. Then
-            the type is to be included in the `cmd` string itself.
-
-            Use capital letter version for integer queue.  ‘b’ or 'B' for
-            before the simulation.  ‘a’ or 'A' for after the simulation.  ‘e’
-            or 'E' for every time step during the simulation.  ‘@’ or '&' for a
-            single command execution at time `time`.  ‘n’ or 'N' for every n’th
-            iteration of the simulation.  ‘i’ or 'I' for a fixed time interval.
-            The command is executed over the period from on to off with
-            intervals of at least dt (the actual intervals will only end at the
-            times of simulation time steps).  ‘x’ for a fixed time multiplier.
-            The command is executed at on, then on+dt, then on+dt*xt, then
-            on+dt*xt2, and so forth.  ‘j’ for every ``dtit`` step with a set
-            starting iteration and stopping iteration.
-
-        kwargs: dict
-            kwargs of :func:`_smoldyn.Command()`.
-
-        """
-        if "step" not in kwargs:
-            kwargs["step"] = self.dt
-        super().addCommand(cmd, cmd_type[0], **kwargs)
-
-    def addCommandStr(self, cmd: str):
-        """Add command using a single string. See the Smoldyn's User Manual for
-        details.
-
-        Parameters
-        ----------
-        cmd : str
-            Command string
-        """
-        super().addCommandStr(cmd)
-
-    # mapping.
-    def addSpecies(
-        self,
-        name: str,
-        state: str = "soln",
-        color: Union[ColorType, Dict[str, ColorType]] = {"soln": "black"},
-        difc: Union[float, Dict[str, float]] = 0.0,
-        display_size: float = 3,
-        mol_list: str = "",
-    ) -> Species:
-        """Add species to Simulation
-
-        See :class:`smoldyn.Species` docs.
-        """
-        # Create a species.
-        s = Species(super(), name, state, color, difc, display_size, mol_list)
-        return s
-
-    def addMolecules(
-        self,
-        species: Species,
-        number: int,
-        pos: List[float] = [],
-        lowpos: List[float] = [],
-        highpos: List[float] = [],
-    ):
-        """See :func:`Species.addToSolution`"""
-        species.addToSolution(number, pos, lowpos, highpos)
-
-    def addSurface(self, name: str, *, panels: List[Panel]) -> Surface:
-        """See :class:`Surface` docs"""
-        return Surface(simulation=super(), name=name, panels=panels)
-
-    def addBidirectionalReaction(
-        self,
-        name: str,
-        subs: List[SpeciesWithState],
-        prds: List[SpeciesWithState],
-        kf: float,
-        kb: float = 0.0,
-        *,
-        binding_radius: float = 0.0,
-        reaction_probability: float = 0.0,
-        compartment: Compartment = None,
-        surface: Surface = None,
-    ) -> BidirectionalReaction:
-
-        return BidirectionalReaction(
-            super(),
-            name,
-            subs,
-            prds,
-            kf,
-            kb,
-            binding_radius=binding_radius,
-            reaction_probability=reaction_probability,
-            compartment=compartment,
-            surface=surface,
-        )
-
-    def addReaction(
-        self,
-        name: str,
-        subs: List[SpeciesWithState],
-        prds: List[SpeciesWithState],
-        *,
-        rate: float = 0.0,
-        compartment: Compartment = None,
-        surface: Surface = None,
-        binding_radius: float = 0.0,
-        reaction_probability: float = 0.0,
-    ) -> Reaction:
-        """Add a reaction (unidirectional)
-
-        See Reaction for details.
-        """
-        return Reaction(
-            super(),
-            name,
-            subs,
-            prds,
-            rate=rate,
-            compartment=compartment,
-            surface=surface,
-            binding_radius=binding_radius,
-            reaction_probability=reaction_probability,
-        )
-
-    def addPartition(self, name: str, value):
-        """Sets the virtual partitions in the simulation volumne. Two
-        specialization is avaiable: :py:class:`MoleculePerBox`, and
-        :py:class:`Box`.
-
-        See also
-        --------
-        :py:class:`MoleculePerBox`
-        :py:class:`Box`
-        """
-        return Partition(super(), name, value)
-
-    def addBox(self, size: float):
-        """See Box.__init__"""
-
-        warnings.warn(
-            "This function is deprecated. Please use setPartitions in the future",
-            DeprecationWarning,
-        )
-        return Box(super(), size)
-
-    def addMoleculePerBox(self, size: float):
-        """See MoleculePerBox.__init__"""
-
-        warnings.warn(
-            "This function is deprecated. Please use setPartitions in the future",
-            DeprecationWarning,
-        )
-        return MoleculePerBox(super(), size)
-
-    def addCompartment(
-        self, name: str, *, surface: Union[str, Surface], point: List[float]
-    ):
-        return Compartment(super(), name, surface=surface, point=point)
-
-    def addOutputData(self, dataname: str) -> None:
-        """Declares the data table called `dataname`, enabling output into it by
-        one or more runtime commands. Spaces are not permitted in the dataname.
-
-        Parameters
-        ----------
-        dataname : str
-            dataname (spaces are not allowed)
-
-        Returns
-        -------
-        None
-
-        """
-        assert " " not in dataname, f"spaces not allowed in dataname: '{dataname}'"
-        r = super().addOutputData(dataname)
-        assert r == _smoldyn.ErrorCode.ok, f"Failed to add output data {r}"
-
-    def getOutputData(self, dataname: str, erase: bool = True) -> List[List[float]]:
-        """Returns data that have been recorded by an observation command (e.g. molcount).
-
-        Parameters
-        ----------
-        dataname : str
-            dataname
-
-        erase: bool
-            When set to `True`, the original data is cleared after a copy  of data
-            is returned to the user.
-
-        Returns
-        -------
-        List[List[float]]
-            A matrix of float.
-        """
-        assert " " not in dataname, f"Must not contain spaces: '{dataname}'"
-        y: List[List[float]] = super().getOutputData(dataname, erase)
-        return y
-
-    def connect(self, func, target, step: int, args: List[float] = []):
-        """Connect a arbitrary Python function to Simulation. The function will
-        be called at every 'step'
-
-        Parameters
-        ----------
-        func :
-            Python function to connect. It must have two arguments. The first
-            argument is always simulation time 't'. the second argument is a
-            list of float which refers to `args` (4th argument of this function)
-        target :
-            Target function or a property. The return value of the connected function
-            i.e., func is the argument to this function.
-        step : int
-            The connected function func is called after these many simulation
-            steps.
-        args : List[float]
-            argument of func (passed by reference). Any change in this list will
-            be visible to func.
-
-        Example
-        -------
-
-        >>> import math
-        >>> s = smoldyn.Simulation(low=(0, 0), high=(10, 10))
-        >>> a = s.addSpecies("a", color="black", difc=0.1)
-        >>> avals = []
-
-        >>> def func(t, args):
-        >>>     global a, avals
-        >>>     x, y = args
-        >>>     avals.append((t, a.difc["soln"]))
-        >>>     return x * math.sin(t) + y
-
-        >>> def target(val):
-        >>>     global a
-        >>>     a.difc = val
-
-        >>> s.connect(func, target, step=10, args=[1, 1])
-        >>> s.run(100, dt=1)
-        >>> avals
-        [(1.0, 0.1),
-         (11.0, 1.8414709848078965),
-         (21.0, 9.793449296524592e-06),
-         (31.0, 1.836655638536056),
-         (41.0, 0.595962354676935),
-         (51.0, 0.841377331195291),
-         (61.0, 1.6702291758433747),
-         (71.0, 0.03388222999160706),
-         (81.0, 1.9510546532543747),
-         (91.0, 0.37011200572554614)]
-        """
-        return super().connect(func, target, step, args)
-
-    def addPath2D(self, *points, closed: bool = False):
-        return Path2D(*points, simulation=super(), closed=closed)
-
-    def addPort(
-        self,
-        *,
-        name: str,
-        surface: Union[Surface, str],
-        panel: str,
-    ):
-        return Port(super(), name=name, surface=surface, panel=panel)
-
-    def addPanel(
-        self,
-        *,
-        name: str = "",
-        shape: _smoldyn.PanelShape = _smoldyn.PanelShape.none,
-        neighbors: List = [],
-    ):
-        return Panel(name=name, shape=shape, neighbors=neighbors, simulation=super())
-
-    def addTriangle(self, *, vertices: Sequence[Sequence[float]] = [[]], name=""):
-        return Triangle(simulation=super(), vertices=vertices, name=name)
-
-    def addRectangle(
-        self,
-        corner: Sequence[float],
-        dimensions: Sequence[float],
-        axis: str,
-        name="",
-    ):
-        return Rectangle(
-            simulation=super(),
-            corner=corner,
-            dimensions=dimensions,
-            axis=axis,
-            name=name,
-        )
-
-    def addSphere(
-        self,
-        *,
-        center: List[float],
-        radius: float,
-        slices: int,
-        stacks: int = 0,
-        name="",
-    ):
-        return Sphere(
-            simulation=super(),
-            center=center,
-            radius=radius,
-            slices=slices,
-            stacks=stacks,
-            name=name,
-        )
-
-    def addHemisphere(
-        self,
-        *,
-        center: List[float],
-        radius: float,
-        vector: List[float],
-        slices: int,
-        stacks: int,
-        name: str = "",
-    ):
-        return Hemisphere(
-            simulation=super(),
-            center=center,
-            radius=radius,
-            vector=vector,
-            slices=slices,
-            stacks=stacks,
-            name=name,
-        )
-
-    def addCylinder(
-        self,
-        *,
-        start: List[float],
-        end: List[float],
-        radius: float,
-        slices: int,
-        stacks: int,
-        name: str = "",
-    ):
-        return Cylinder(
-            simulation=super(),
-            start=start,
-            end=end,
-            radius=radius,
-            slices=slices,
-            stacks=stacks,
-            name=name,
-        )
-
-    def addDisk(
-        self,
-        *,
-        center: List[float],
-        radius: float,
-        slices: int,
-        vector: List[float],
-        name="",
-    ):
-        return Disk(
-            simulation=super(),
-            center=center,
-            radius=radius,
-            slices=slices,
-            vector=vector,
-            name=name,
-        )
+"""Smoldyn user API.
+"""
+
+__author__ = "Dilawar Singh"
+__email__ = "dilawar.s.rajput@gmail.com"
+
+__all__ = [
+    "__version__",
+    "version",
+    "getError",
+    "Simulation",
+    "Species",
+    "Panel",
+    "Triangle",
+    "Rectangle",
+    "Sphere",
+    "Hemisphere",
+    "Cylinder",
+    "Disk",
+    "Path2D",
+    "Surface",
+    "Port",
+    "Partition",
+    "Compartment",
+    "Reaction",
+    "BidirectionalReaction",
+]
+
+import operator
+import functools
+import math
+import warnings
+from pathlib import Path
+from dataclasses import dataclass
+
+from typing import Union, Tuple, List, Dict, Optional, Sequence
+
+
+from smoldyn.types import Color, BoundType, ColorType, DiffConst
+from smoldyn import _smoldyn
+
+# Path of model file.
+# It does not look like there is a beter way to find this path out
+# automatically. This is needed by simptr.
+import inspect
+
+__top_model_file__ = Path(inspect.stack()[-1].filename)
+
+# Logger
+import logging
+
+__logger__ = logging.getLogger(__name__)
+ch = logging.StreamHandler()
+ch.setLevel(logging.WARNING)
+ch.setFormatter(logging.Formatter("%(name)s - %(levelname)s - %(message)s"))
+__logger__.addHandler(ch)
+
+
+def version():
+    """Get version"""
+    return _smoldyn.__version__
+
+
+# alias of version()
+__version__: str = version()
+
+
+def getError(clear: bool = False) -> Tuple[_smoldyn.ErrorCode, str]:
+    return _smoldyn.getError(clear)
+
+
+def _toMS(st: Union[str, _smoldyn.MolecState]) -> _smoldyn.MolecState:
+    """Convert a string to equivalent MolecState.
+
+    Parameters
+    ----------
+    st : Tuple[str, _smoldyn.MolecState]
+        Given state either a string or MolecState. If MolecState is given, this
+        function simply returns it.
+    """
+    return _smoldyn.MolecState.__members__[st] if isinstance(st, str) else st
+
+
+class Species(object):
+    def __init__(
+        self,
+        simulation: _smoldyn.Simulation,
+        name: str,
+        state: str = "soln",
+        color: Union[ColorType, Dict[str, ColorType]] = {"soln": "black"},
+        difc: Union[float, Dict[str, float]] = 0.0,
+        display_size: float = 3,
+        mol_list: str = "",
+    ):
+        """
+        Species or Molecule.
+
+        Parameters
+        ----------
+        name : str
+            Name of the species.
+        state : str
+            State of the species. One of the following:
+                'soln', 'front', 'back', 'up', 'down', 'bsoln', 'all', 'none','some'
+        color: Color or dict of Colors
+            If a single :py:class:`Color` is given, all states of this molecule will be
+            assigned this color. To assign different colors to different
+            states, use a dictionary of :py:class:`Color`.
+        difc : float or a dict of floats
+            Diffusion coefficient. If a single value is given, all states of
+            the molecule gets the same value. To assign different values to
+            different states, use a dict e.g. {'soln':1, 'front':2}.
+        display_size : float, optional
+            display size of the molecule. For the ``opengl`` graphics method, the
+            this value is in pixels.  Here, numbers from 2 to 4 are
+            typically good choices (default 3px).  For better graphics
+            options (opengl_good and opengl_better), the display size value is
+            the radius with which the molecule is drawn, using the same units
+            as elsewhere in the input file.
+        mol_list : str, optional
+            molecule list (default '')
+
+        """
+        self.simulation = simulation
+        self.name: str = name
+        assert self.name
+
+        self._displaySize: Dict[str, float] = {}
+        self._color: Dict[str, Color] = {}
+        self._difc: Dict[str, float] = {}
+        self._mol_list: str = ""
+
+        k = self.simulation.addSpecies(self.name)
+        assert k == _smoldyn.ErrorCode.ok, f"Failed to add molecule {k}"
+
+        if state not in _smoldyn.MolecState.__members__:
+            raise NameError(
+                f"{state} is not a valid MolecState. Available "
+                "states are:{', '.join(_smoldyn.MolecState.__members__.keys())}"
+            )
+
+        self.state = state
+
+        # Prepare diffusion constant dict (for state).
+        if not isinstance(difc, dict):
+            difc = {self.state: difc}
+        self.difc = difc
+
+        # assign color
+        self.color = color
+        self.display_size = display_size
+        if mol_list:
+            self.mol_list: str = mol_list
+
+    def __repr__(self):
+        return f"<Molecule: {self.name}, difc={self.difc}, state={self.state}>"
+
+    def __to_disp__(self):
+        return f"{self.name}({self.state})"
+
+    def setStyle(
+        self,
+        display_size: Union[float, Dict[str, float]],
+        color: Union[ColorType, Dict[str, ColorType]],
+    ):
+        self.color = color
+        self.display_size = display_size
+
+    @property
+    def difc(self) -> DiffConst:
+        return self._difc
+
+    @difc.setter
+    def difc(self, difconst: DiffConst):
+        """Isotropic Diffusion coeffiecient of the Species.
+
+        Parameters
+        ----------
+        difconst : DiffConst (default '0')
+            If a single value is given, all states of the
+            molecule are assigned the same value. To assign state specific
+            values, use a dictionary. Missing states will be assigned 0.0.
+        """
+        self._difc = (
+            {self.state: difconst} if not isinstance(difconst, dict) else difconst
+        )
+        for state, D in self._difc.items():
+            st = (
+                _smoldyn.MolecState.__members__[state]
+                if isinstance(state, str)
+                else state
+            )
+            k = self.simulation.setSpeciesMobility(self.name, st, D)
+            assert k == _smoldyn.ErrorCode.ok
+
+    @property
+    def mol_list(self) -> str:
+        return self._mol_list
+
+    @mol_list.setter
+    def mol_list(self, val):
+        k = self.simulation.addMolList(val)
+        assert k == _smoldyn.ErrorCode.ok, f"Failed to add mollist: {k}"
+        k = self.simulation.setMolList(self.name, _toMS(self.state), val)
+        assert (
+            k == _smoldyn.ErrorCode.ok
+        ), f"Failed to set mol_list={val} on {self}: {k}"
+        self._mol_list = val
+
+    @property
+    def color(self):
+        return self._color
+
+    @color.setter
+    def color(self, clr: Union[ColorType, Color]):
+        self._color = {self.state: Color(clr)} if not isinstance(clr, dict) else clr
+        for state, _clr in self._color.items():
+            k = self.simulation.setMoleculeColor(
+                self.name, _toMS(state), Color(_clr).rgba
+            )
+            assert k == _smoldyn.ErrorCode.ok
+
+    @property
+    def display_size(self):
+        return self._displaySize
+
+    @display_size.setter
+    def display_size(self, size: Union[float, Dict[str, float]]):
+        """Set the display_size of the molecule.
+
+        Parameters
+        ----------
+        size : Union[float, Dict[str, float]]
+            If a single value is provided, it is applied to all states of the
+            moelcule. For state specific value of display_size, use a
+            dictionary.
+
+        Note
+        -----
+        For the “opengl” graphics level, the display size value is in pixels.
+        Here, numbers from 2 to 4 are typically good choices (deafult 2px).
+        For the two better graphics options, the display size value is the
+        radius with which the molecule is drawn, using the same units as
+        elsewhere in the input file.
+        """
+        if isinstance(size, (float, int)):
+            size = {_smoldyn.MolecState.all: size}
+        self._displaySize = size
+        for state, size in self._displaySize.items():
+            state = (
+                _smoldyn.MolecState.__members__[state]
+                if isinstance(state, str)
+                else state
+            )
+            k = self.simulation.setMoleculeSize(self.name, state, size)
+            assert k == _smoldyn.ErrorCode.ok
+
+    def addToSolution(
+        self,
+        N: int,
+        pos: List[float] = [],
+        highpos: List[float] = [],
+        lowpos: List[float] = [],
+    ):
+        """Add molecule to solution.
+
+        Parameters
+        ----------
+        N : float
+            Number of molecules
+        pos : List[float]
+            Fixed location. If given, both `lowpos` and `highpos` will be set
+            to this value.
+        highpos : List[float]
+            Upper bound on the molecules location. Molecules will be distributed
+            uniformly between the lowerbound and this value.
+        lowpos : List[float]
+            Lower bound on the molecules location. Molecules will be distributed
+            uniformly between the upper bound and this value.
+        """
+        assert (
+            self.state == "soln"
+        ), f"You can't use this function on a Species with type {self.state}"
+        if pos:
+            lowpos = highpos = pos
+        k = self.simulation.addSolutionMolecules(self.name, N, lowpos, highpos)
+        assert k == _smoldyn.ErrorCode.ok, f"Failed to add to solution: {k}"
+
+
+@dataclass
+class NullSpecies(Species):
+    name: str = ""
+    state = _smoldyn.MolecState.__members__["none"]
+
+    def __bool__(self):
+        return False
+
+    def __len__(self):
+        return 0
+
+
+# Type of a substract and product of a Reaction
+SpeciesState = Union[_smoldyn.MolecState, str]
+SpeciesWithState = Union[Species, Tuple[Species, SpeciesState]]
+
+
+class Panel(object):
+    def __init__(
+        self,
+        *,
+        name: str = "",
+        shape: _smoldyn.PanelShape = _smoldyn.PanelShape.none,
+        neighbors: List["Panel"] = [],
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Panels are components of a surface. One or more Panels are requried
+        to form a Surface. Following geometric primitives are available.
+
+        - [Rectangle](smoldyn.smoldyn.Rectangle)
+        - [Triangle](smoldyn.smoldyn.Triangle)
+        - [Sphere](smoldyn.smoldyn.Sphere)
+        - [Hemisphere](smoldyn.smoldyn.Hemisphere)
+        - [Cylinder](smoldyn.smoldyn.Cylinder)
+        - [Disk](smoldyn.smoldyn.Disk)
+        """
+
+        # self._neighbors: List[Panel] = []
+        self._neighbors: List = []
+        self.name = name
+        self.ctype: _smoldyn.PanelShape = shape
+        self.pts: List[float] = []
+        self.simulation = simulation
+        self.front = _PanelFace(name="front", panel=self, simulation=self.simulation)
+        self.back = _PanelFace(simulation=self.simulation, name="back", panel=self)
+        self.surface: Surface = NullSurface()
+        self.neighbors = neighbors
+
+    def _setSimulation(self, simulation: _smoldyn.Simulation):
+        assert simulation
+        self.simulation = simulation
+        self.front.simulation = simulation
+        self.back.simulation = simulation
+
+    def jumpTo(self, face1: str, panel2, face2: str, bidirectional: bool = False):
+        """Add a jump reaction between two panels of the same surface.
+
+        This panel has name panel1, and face face1.  A molecule that hits this
+        face of the panel, and that has “jump” action for this face, gets
+        translated to the face face2 of the panel panel2 (which needs to be the
+        same shape as the originating panel).
+
+        Parameters
+        ----------
+        face1 : Panel
+
+        panel2 : to this Panel
+        face2 : to this face
+
+        Examples
+        --------
+
+        Smoldyn expression:
+            jump r1 front <-> r2 front
+
+        >>> r1.addJump('front', r2, 'front', True)
+
+        Or,
+
+        >>> r1.front.jumpTo(r2.front, True)
+        """
+        jfrom = getattr(self, face1)
+        assert jfrom, f"Could not locate {face1} on {self}."
+        assert isinstance(jfrom, _PanelFace)
+        jto = getattr(panel2, face2)
+        assert jto, f"Could not locate {face2} on {panel2}."
+        assert isinstance(jto, _PanelFace)
+
+        return jfrom.jumpTo(jto, bidirectional)
+
+    def __str__(self):
+        return f"<{self.name} type={self.ctype} index={self.index} points={self.pts}>"
+
+    def _axisIndex(self, axisname: str):
+        axisDict = dict(x=0, y=1, z=2)
+        return int(axisDict.get(axisname.lower(), axisname))
+
+    @property
+    def index(self) -> int:
+        assert self.simulation
+        v: int = self.simulation.getPanelIndexNT(self.surface.name, self.name)
+        return v
+
+    def toText(self):
+        return f"panel {self.ctype} {self.axisstr} {' '.join(map(str,self.pts))} {self.name}".strip()
+
+    @property
+    def neighbors(self):
+        return self._neighbors
+
+    @neighbors.setter
+    def neighbors(self, panels: List):
+        self._neighbors = panels
+        for panel in panels:
+            self._assignNeighbor(panel)
+
+    @property
+    def neighbor(self):
+        return self._neighbors[0]
+
+    @neighbor.setter
+    def neighbor(self, panel):
+        self._assignNeighbor(panel)
+
+    def _assignNeighbor(self, panel, reciprocal: bool = False):
+        assert self.surface, f"Panel {self} has no Surface assigned."
+        assert panel.surface, f"Panel {panel} has no Surface assigned."
+        assert self != panel, "A panel cannot be its own neighbor"
+        assert self.simulation
+        k = self.simulation.addPanelNeighbor(
+            self.surface.name, self.name, panel.surface.name, panel.name, reciprocal
+        )
+        assert k == _smoldyn.ErrorCode.ok
+
+    def _getName(self, index: int) -> str:
+        if self.name:
+            return self.name
+        return f"{self.ctype}{index}"
+
+    def setNeighbors(self, panels, reciprocal: bool = False):
+        """Set neighbors.
+
+        Parameters
+        ----------
+        panels :
+            Neighboring panels
+        reciprocal : bool
+            If True, this panel also becomes neighbor of all panels in arguments.
+
+        See Also
+        --------
+        Panel.neighbor, Panel.neighbors
+        """
+        for panel in panels:
+            self._assignNeighbor(panel, reciprocal)
+
+
+class Rectangle(Panel):
+    def __init__(
+        self,
+        corner: Sequence[float],
+        dimensions: Sequence[float],
+        axis: str,
+        name: str = "",
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Rectangle
+
+        Parameters
+        ----------
+        corner :
+            One corner of the rectangle.
+        dimensions :
+            Dimensions of the rectangle e.g., for a 2D rectangle it is a list of
+            values of width and height.
+        height : float
+            height of the rectangle
+        axis : str
+            axis perpendicular to the rectangle preceded by '+' if the panel
+            front faces the positive axis and '-' if it faces the negative
+            axis e.g., '+x', '+0', '-y' etc.
+        name : optional
+            name of the panel.
+        """
+        super().__init__(
+            simulation=simulation, shape=_smoldyn.PanelShape.rect, name=name
+        )
+        self.corner = corner
+        self.dimensions = dimensions
+        assert axis[0] in "+-", "axis must precede by '+' or '-'"
+        assert axis[1].lower() in "012xyz"
+        self.axis = axis.lower()
+        self.axisIndex = self._axisIndex(axis[1])
+        self.toGenericPanel()
+
+    def toGenericPanel(self):
+        self.axisstr = self.axis
+        self.pts = [*self.corner, *self.dimensions]
+        return self.axisstr, self.pts
+
+
+class Triangle(Panel):
+    def __init__(
+        self,
+        *,
+        vertices: Sequence[Sequence[float]] = [[]],
+        name: str = "",
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Triangle Panel.
+
+        Parameters
+        ----------
+        vertices :
+            vertices of triangle.
+        name :
+            name
+        """
+        super().__init__(
+            simulation=simulation, shape=_smoldyn.PanelShape.tri, name=name
+        )
+        self.axisstr = ""
+        self.vertices = vertices
+        self.pts = functools.reduce(operator.iconcat, vertices, [])
+
+
+class Sphere(Panel):
+    def __init__(
+        self,
+        *,
+        center: List[float],
+        radius: float,
+        slices: int,
+        stacks: int = 0,
+        name: str = "",
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Sphere
+
+        Parameters
+        ----------
+        center :
+            The center of the sphere.
+        radius : float
+            The radius of the sphere.
+        slices: int
+            Number of slices (longitudnal lines) that are used for drawing the sphere.
+        stacks: int
+            Number of stacks (latitude lines, default 0) that are used to drawing the sphere. `
+            If a non-postive number is given,`slices` value is used.
+        name : optional
+            name of the panel. If omitted, 0, 1, 2 etc. will be assigned.
+        """
+        super().__init__(
+            simulation=simulation, shape=_smoldyn.PanelShape.sph, name=name
+        )
+        self.center = center
+        self.radius = radius
+        self.slices = slices
+        assert self.slices > 0, "Positive int is required"
+        self.stacks = stacks if stacks > 0 else slices
+        # Smoldyn panel
+        self.axisstr = ""
+        self.pts = [*self.center, self.radius, self.slices, self.stacks]
+
+
+class Hemisphere(Panel):
+    def __init__(
+        self,
+        *,
+        center: List[float],
+        radius: float,
+        vector: List[float],
+        slices: int,
+        stacks: int,
+        name: str = "",
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Hemisphere
+
+        Parameters
+        ----------
+        center :
+            The center of hemisphere
+        radius : float
+            The radius of the hemisphere. Enter a positive radius to have the
+            front of the surface on the outside and a negative radius for it to
+            be on the inside.
+        vector :
+            The outward pointing vector (needs NOT be normalized)
+        slices : int
+            The number of slices
+        stacks : int
+            The number of stacks
+        name : optional
+            name
+        """
+        super().__init__(
+            simulation=simulation, shape=_smoldyn.PanelShape.hemi, name=name
+        )
+        self.center = center
+        self.radius = radius
+        self.vector = vector
+        self.slices = slices
+        self.stacks = stacks
+        # Smoldyn Panel
+        self.axisstr = ""
+        self.pts = [*self.center, self.radius, *self.vector, self.slices, self.stacks]
+
+
+class Cylinder(Panel):
+    def __init__(
+        self,
+        *,
+        start: List[float],
+        end: List[float],
+        radius: float,
+        slices: int,
+        stacks: int,
+        name: str = "",
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Cylinder
+
+        Parameters
+        ----------
+        start :
+            Cylinder axis start point
+        end :
+            Cylinder axis's end point
+        radius : float
+            The radius of the cylinder. If the radius is negative then the front
+            of the surface is on the inside otherwise it is on the outside.
+        slices : int
+            Number of slices
+        stacks : int
+            Number of stacks
+        name : optional
+            name
+        """
+        super().__init__(
+            simulation=simulation, shape=_smoldyn.PanelShape.cyl, name=name
+        )
+        self.start: List[float] = start
+        self.end: List[float] = end
+        self.radius: float = radius
+        self.slices: int = slices
+        self.stacks: int = stacks
+        # Smoldyn panel
+        self.axisstr: str = ""
+        self.pts = [*self.start, *self.end, self.radius, self.slices, self.stacks]
+
+
+class Disk(Panel):
+    def __init__(
+        self,
+        *,
+        center: List[float],
+        radius: float,
+        slices: int,
+        vector: List[float],
+        name="",
+        simulation: Optional[_smoldyn.Simulation] = None,
+    ):
+        """Disk
+
+        Parameters
+        ----------
+        center :
+            center of the disk.
+        radius : float
+            radius of the disk.
+        slices : int
+            Number of slices for drawing.
+        vector:
+            A vector that points away from the front of the disk. The size of
+            this vector is 2 for 2-D and 3 for 3-D.
+        name: optional
+            name of this Disk.
+        """
+        super().__init__(
+            simulation=simulation, shape=_smoldyn.PanelShape.disk, name=name
+        )
+        assert slices > -1, f"Slices must be positive. Given value {slices}"
+        self.center = center
+        self.radius = radius
+        self.slices = slices
+        self.vector = vector
+        # Smoldyn panel
+        self.axisstr = ""
+        # From the manual: #Slice is entered last (after normal vector).
+        self.pts = [*self.center, self.radius, *self.vector, self.slices]
+
+
+class _PanelFace(object):
+    def __init__(self, *, simulation: _smoldyn.Simulation, name: str, panel: Panel):
+        self.simulation = simulation
+        assert name in ["front", "back"]
+        self.name = _smoldyn.PanelFace.__members__[name]
+        self.panel = panel
+
+    def jumpTo(self, toface, bidirectional: bool = False):
+        """Add a jump reaction between two panels of same Surface
+
+        See also
+        --------
+        Panel.jumpTo
+        """
+        assert (
+            self.panel.ctype == toface.panel.ctype
+        ), "Both panels must have same geometry"
+        assert (
+            self.panel.surface == toface.panel.surface
+        ), "Both panels must have same surface"
+        __logger__.debug(
+            f"{self.panel.surface.name}, {self.panel.name} "
+            f", {self.name}, {toface.panel.name}, {toface.name}, "
+            f"{bidirectional}"
+        )
+        k = self.simulation.setPanelJump(
+            self.panel.surface.name,
+            self.panel.name,
+            self.name,
+            toface.panel.name,
+            toface.name,
+            bidirectional,
+        )
+        assert k == _smoldyn.ErrorCode.ok
+
+
+class _SurfaceFaceCollection(object):
+    def __init__(
+        self, simulation: _smoldyn.Simulation, faces: List[str], surfname: str
+    ):
+        """Collection of faces of a surface"""
+        self.simulation = simulation
+        self.faces: List[str] = faces
+        self.surfname: str = surfname
+        self.__valid_actions_ = [
+            "reflect",
+            "trans",
+            "absorb",
+            "jump",
+            "port",
+            "mult",
+            "no",
+            "none",
+        ]
+
+    def setStyle(
+        self,
+        color: ColorType = "",
+        drawmode: str = "none",
+        thickness: float = 1.0,
+        stipplefactor: int = -1,
+        stipplepattern: int = -1,
+        shininess: int = -1,
+    ):
+        """Set drawing style for the face of surface.
+
+        Parameters
+        ----------
+        drawmode : str
+            May be "none", "vertex", "edge", "face", or combinations of ‘v’,
+            ‘e’, or ‘f’ for multiple renderings of vertices, edges, and/or
+            faces. 2-D spheres and hemispheres are either filled or are
+            outlined depending on the polygon frontcharacter. If multiple
+            renderings are chosen in 3D, then panel faces are shown in the
+            requested color and other renderings are shown in black.
+        thickness : float
+            Boldness of the surface in pixels for drawing purposes.  This is
+            only relevant for 1-D and 2-D simulations, and for 3-D simulations
+            in which surfaces are drawn with just vertices or edges and not
+            faces.
+        color : Color
+            color e.g. 'black', 'red', [0.1,0.1,0.1] etc.
+        stipplefactor : int
+            stipplefactor is the repeat distance for the entire stippling
+            pattern (1 is a good choice).  Stippling of the surface edges, for
+            drawing purposes.  This is only relevant for 3-D simulations in
+            which surfaces are drawn with just edges and not faces, and with
+            opengl_good or opengl_better display method.
+        stipplepattern : int
+            stipplepattern a hexidecimal integer, enter the stippling pattern between
+            ``0x0000`` (0) and ``0xFFFF`` (65536), ``0x00FF`` (256) has long dashes,
+            ``0x0F0F`` (3855) has medium dashes, ``0x5555`` (21845)  has dots, etc.
+            Turn stippling off with ``0xFFFF`` (65536).
+        shininess : float
+            Shininess of the surface for drawing purposes.  This value can
+            range from 0 for visually flat surfaces to 128 for very shiny
+            surfaces.  This is only relevant for some simulations.
+        """
+        for which in self.faces:
+            # TODO : Check on drawmode
+            k = self.simulation.setSurfaceStyle(
+                self.surfname,
+                _smoldyn.PanelFace.__members__[which],
+                _smoldyn.DrawMode.__members__[drawmode],
+                thickness,
+                Color(color).rgba,
+                stipplefactor,
+                stipplepattern,
+                shininess,
+            )
+            assert k == _smoldyn.ErrorCode.ok, f"Failed to set drawing style {k}"
+
+    def setAction(
+        self,
+        species: Union[Species, List[Species]],
+        action: str,
+        new_species: Optional[Species] = None,
+    ):
+        """The behavior of molecules named species when they collide with this
+        face of this surface.
+
+        Parameters
+        ----------
+        species :
+            List of species or a single species. DO NOT use the name of
+            species.
+        action : str
+            The action can be  `“reflect”`, `“absorb”`, `“transmit”`, `“jump”`,
+            `“port”`, or `“periodic”`.
+        new_species:
+            TODO: Implement it.
+            If `new_species` is entered, then the molecule changes to this new
+            species upon surface collision. In addition, it’s permissible to
+            enter the action as “multiple,” in which case the rates need to be
+            set with rate; alternatively, just setting the rates will
+            automatically set the action to “multiple.” The default is
+            transmission for all molecules.
+        """
+        assert (
+            action in self.__valid_actions_
+        ), f"'{action}' is not a valid action. Available actions: {', '.join(self.__valid_actions_)}"
+
+        if isinstance(species, str):
+            raise NameError(
+                "This API does not accepts species by their names or the keyword 'all'."
+                " Please pass the objects."
+            )
+        listSpecies = [species] if isinstance(species, Species) else species
+        for sp in listSpecies:
+            if isinstance(sp, Species):
+                sname, sstate = sp.name, sp.state
+            else:
+                sname, sstate = sp, _smoldyn.MolecState.soln
+
+            if isinstance(sstate, str):
+                sstate = _smoldyn.MolecState.__members__[sstate]
+
+            # TODO: see issue #17
+            if new_species:
+                raise NotImplementedError("This feature is not implemented.")
+
+            for which in self.faces:
+                k = self.simulation.setSurfaceAction(
+                    self.surfname,
+                    _smoldyn.PanelFace.__members__[which],
+                    sname,
+                    sstate,
+                    _smoldyn.SrfAction.__members__[action],
+                )
+                assert k == _smoldyn.ErrorCode.ok, f"Failed setSurfaceAction: {k}"
+
+
+class Path2D(object):
+    def __init__(self, *points, simulation: _smoldyn.Simulation, closed: bool = False):
+        """Construct a 2D path from given points.
+
+        A Path2D consists of `Rectangle` and `Triangle`.
+
+        Parameters
+        ----------
+        *points:
+            Points
+        simulation:
+            _smoldyn.Simulation object.
+        closed: bool
+            If closed is `True`, the last point and the first point are
+            connected. Default `False`.
+        """
+        self.points = list(points)
+
+        self.simulation = simulation
+        assert self.simulation
+
+        if closed and self.points[0] != self.points[-1]:
+            self.points.append(self.points[0])
+        self.panels: List[Panel] = []
+        for p1, p2 in zip(self.points, self.points[1:]):
+            (x1, y1), (x2, y2) = p1, p2
+            theta = math.atan2(y2 - y1, x2 - x1)
+            __logger__.debug(f"theta={theta} {p1} and {p2}")
+            if theta in [0.0, math.pi, math.pi / 2.0, -math.pi / 2.0]:
+                if theta == 0.0:
+                    axis = "+y"
+                elif theta == math.pi:
+                    axis = "-y"
+                elif theta == math.pi / 2.0:
+                    axis = "-x"
+                elif theta == -math.pi / 2.0:
+                    axis = "+x"
+                else:
+                    raise RuntimeError(
+                        "Should not be here."
+                        " Python3 numerical computation is broken!"
+                    )
+                length = x2 - x1 if y2 == y1 else y2 - y1
+                p = Rectangle(
+                    simulation=self.simulation,
+                    corner=(x1, y1),
+                    dimensions=[length],
+                    axis=axis,
+                )
+                __logger__.info(f"Added a Rectangle {p}")
+                self.panels.append(p)
+            else:
+                t = Triangle(simulation=self.simulation, vertices=((x1, y1), (x2, y2)))
+                self.panels.append(t)
+
+
+# TODO: Add a Path3D or Surface3D. not sure what to call it.
+
+
+class Surface(object):
+    """Surfaces are infinitesimally thin structures that can be used to
+    represent cell membranes, obstructions, system boundaries, or other things.
+
+    Note
+    ----
+
+    They are 2D structures in 3D simulations, or 1D lines or curves in 2D simulations (or 0D points
+    in 1D simulations).Each surface has a “front” and a “back” face, so molecules can interact
+    differently with the two sides of a surface.Each surface is composed of one or more
+    “:py:class:`~Panels`”, where each panels can be a rectangle, triangle, sphere, hemisphere,
+    cylinder, or a disk. Surfaces can be disjoint, with separate non-connected portions.  However,
+    all portions of a given surface type are displayed in the same way and interact with molecules
+    in the same way.
+
+    """
+
+    def __init__(
+        self, *, simulation: _smoldyn.Simulation, name: str, panels: List[Panel]
+    ):
+        """
+        Parameters
+        ----------
+        simulation:
+            Simulation object
+        panels : List[Panel]
+            List of panels. A surface must have at least one.
+        name : str
+            name of the surface
+
+        Examples
+        --------
+        >>> r1 = S.Rectangle(corner=[100,0,0], dimensions=[100,100], axis='-x')
+        >>> r2 = S.Rectangle(corner=[0,0,0], dimensions=[100,100], axis='+y')
+        >>> s = smoldyn.Surface("walls", panels=["r1", "r2"])
+        """
+        self.simulation = simulation
+        assert self.simulation
+
+        self.panels = panels
+        self.name = name
+        self.simulation.addSurface(self.name)
+
+        self.front = _SurfaceFaceCollection(self.simulation, ["front"], name)
+        self.back = _SurfaceFaceCollection(self.simulation, ["back"], name)
+        self.both = _SurfaceFaceCollection(self.simulation, ["front", "back"], name)
+        self._addPanelsToSmoldyn()
+
+    def _addPanelsToSmoldyn(self):
+        """Call libsmodyn API to construct this surface' Panels"""
+        assert self.name, "Surface name is missing"
+        for i, panel in enumerate(self.panels):
+            panel.name = panel._getName(i)
+            panel.surface = self
+
+            # Set simulation object before adding Panel.
+            panel._setSimulation(self.simulation)
+
+            # Add panels.
+            k = self.simulation.addPanel(
+                self.name,
+                panel.ctype,
+                panel.name,
+                panel.axisstr,
+                panel.pts,
+            )
+            assert (
+                k == _smoldyn.ErrorCode.ok
+            ), f"Failed to add panel (error={k}): Surface:{self.name} {panel}"
+
+    def setStyle(self, face, *args, **kwargs):
+        """See the function :func:`_SurfaceFaceCollection.setStyle` for more
+        details. This function forwards arguments to
+        :func:`_SurfaceFaceCollection.setStyle`.
+
+        Parameters
+        ----------
+        face: str
+            face of the surface: 'front', 'back', 'both'
+        *args:
+            See :func:`_SurfaceFaceCollection.setStyle`
+        **kwargs:
+            See :func:`_SurfaceFaceCollection.setStyle`
+
+        See Also
+        --------
+        :func:`_SurfaceFaceCollection.setStyle`
+        """
+        assert face in ["front", "back", "both"]
+        getattr(self, face).setStyle(*args, **kwargs)
+
+    def setAction(
+        self,
+        face: str,
+        species: Union[Species, List[Species]],
+        action: str,
+        new_species: Optional[Species] = None,
+    ):
+        """Set drawing style for the face of surface
+        (calls :func:`_SurfaceFaceCollection.setAction`)
+
+        Parameters
+        ----------
+        face: str
+            face of the surface: 'front', 'back', 'both'
+        species :
+            List of species or a single species. DO NOT use the name of
+            species.
+        action : str
+            The action can be  `“reflect”`, `“absorb”`, `“transmit”`, `“jump”`,
+            `“port”`, or `“periodic”`.
+        new_species:
+            TODO: Implement it.
+            If `new_species` is entered, then the molecule changes to this new
+            species upon surface collision. In addition, it’s permissible to
+            enter the action as “multiple,” in which case the rates need to be
+            set with rate; alternatively, just setting the rates will
+            automatically set the action to “multiple.” The default is
+            transmission for all molecules.
+
+
+        See Also
+        --------
+        :func:`_SurfaceFaceCollection.setAction`
+        """
+        getattr(self, face).setAction(species, action, new_species)
+
+    def addMolecules(
+        self,
+        species: SpeciesWithState,
+        N: int,
+        panels: Optional[List[Panel]] = None,
+        pos: List[float] = [],
+    ):
+        """Place molecules with random or specific positions onto a given
+        surface (optionally specified panels).
+
+        Parameters
+        ----------
+        species:
+            Species to add, a Species or a tuple of (Species, MolecState)
+            e.g. (A, 'front')
+        N : int
+            number of molecules
+        surface : smoldyn.geometry.Surface
+            Surface
+        panels: smoldyn.geometry.Panel
+            Panels of surface. If `None` is given then all panels of
+            surfece are used.
+        pos: List[float]
+            Position of the molecules. If not given, then randomly distribute
+            the molecules onto the surface/panels.
+        """
+        assert N > 0, "Expected a positive number"
+        assert species
+        if isinstance(species, Species):
+            sname = species.name
+            sstate = species.state
+        else:
+            assert len(species) == 2, "Expected tuple of (Species, MolecState)"
+            sname = species[0].name
+            sstate = _toMS(species[1])
+
+        panels = panels if panels is not None else self.panels
+
+        # Distribute molecules equally among the panels.
+        _N = N // len(panels)
+        Ns = [_N] * len(panels)
+        Ns[0] += N - sum(Ns)
+        assert sum(Ns) == N
+
+        for panel, _n in zip(panels, Ns):
+            assert panel
+            assert panel.ctype
+            k = self.simulation.addSurfaceMolecules(
+                sname,
+                sstate,
+                _n,
+                self.name,
+                panel.ctype,
+                panel.name,
+                pos,
+            )
+            assert k == _smoldyn.ErrorCode.ok, k
+
+    def _setRate(
+        self,
+        species: SpeciesWithState,
+        state1: SpeciesState,
+        state2: SpeciesState,
+        rate: float,
+        new_species: Optional[Species] = None,
+        isinternal: bool = False,
+    ):
+        if not isinstance(species, Species):
+            sname, sstate = species[0].name, species[1]
+        else:
+            sname, sstate = species.name, species.state
+        state1 = _toMS(state1)
+        new_species_str = new_species.name if new_species else ""
+        k = self.simulation.setSurfaceRate(
+            self.name,
+            sname,
+            _toMS(sstate),
+            _toMS(state1),
+            _toMS(state2),
+            rate,
+            new_species_str,
+            isinternal,
+        )
+        assert k == _smoldyn.ErrorCode.ok, "Failed to set rate"
+
+    def setRate(
+        self,
+        species: SpeciesWithState,
+        state1: SpeciesState,
+        state2: SpeciesState,
+        rate: float,
+        revrate: float = 0.0,
+        new_species: Optional[Species] = None,
+        isinternal: bool = False,
+    ):
+        """The rate constant for transitions from `state1` to `state2` of molecules
+        named `species`.
+
+        Parameters
+        ----------
+        species : SpeciesWithState
+            A species or a tuple of `Species` and its state.
+        state1 : SpeciesState
+            Can be any of: fsoln, bsoln (in solution, hitting the front or
+            back of the panel, respectively), front, back, up, or down.
+        state2 : SpeciesState
+            Can be any of: fsoln, bsoln (in solution, hitting the front or
+            back of the panel, respectively), front, back, up, or down.
+        rate : float
+            rate (must be on-zero positive value).
+        revrate: float
+            reverse rate (default 0.0). If this value is a positive non-zero
+            value, then a reverse rate is also set.
+        new_species :
+            newspecies
+        isinternal:
+            When set to `True`, a different value is entered. Instead of
+            entering the surface action rate, enter the probability of the
+            action at each collision.  Probabilities for reflection are ignored
+            since they are calculated as the probability that the molecule does
+            not transmit, absorb, or jump.
+        """
+        self._setRate(species, state1, state2, rate, new_species, isinternal)
+        if revrate > 0.0:
+            self._setRate(species, state2, state1, revrate, new_species, isinternal)
+
+
+class NullSurface(Surface):
+    def __init__(self):
+        self.name = ""
+        self.panels = []
+
+    def __bool__(self):
+        return False
+
+
+class Port(object):
+    """Ports are data structures that are used for importing and
+    exporting molecules between a Smoldyn simulation and another simulation.  In
+    particular, they are designed for the incorporation of Smoldyn into MOOSE,
+    but they could also be used to connect multiple Smoldyn simulations or for
+    other connections.
+
+    A port is essentially a surface and a buffer. Smoldyn
+    molecules that hit the porting surface are removed from the Smoldyn
+    simulation and are put into the buffer for export.  Once exported, they are
+    removed from the buffer.  Also, molecules may be added to the Smoldyn
+    simulation at the porting surface by other programs.
+    """
+
+    def __init__(
+        self,
+        simulation: _smoldyn.Simulation,
+        *,
+        name: str,
+        surface: Union[Surface, str],
+        panel: str,
+    ):
+        """
+        Parameters
+        ----------
+        simulation:
+            _smoldyn.Simulation() object
+        name : str
+            name of the port
+        surface : Union[Surface,str]
+            Porting surface (must be created before).
+        panel : str
+            Face of the which surface active for porting: "front" or "back".
+        """
+        self.simulation = simulation
+        self.name: str = name
+        self.surfname = surface.name if isinstance(surface, Surface) else surface
+        assert panel in ["front", "back"]
+        self.panel = _smoldyn.PanelFace.__members__[panel]
+        k = self.simulation.addPort(self.name, self.surfname, self.panel)
+        assert k == _smoldyn.ErrorCode.ok
+
+
+class Compartment(object):
+    def __init__(
+        self,
+        simulation: _smoldyn.Simulation,
+        name: str,
+        *,
+        surface: Union[str, Surface],
+        point: List[float],
+    ):
+        """Comapartment.
+
+        Parameters
+        ----------
+        name : str
+            name of the compartment.
+        surface : Union[str, Surface]
+            Name of the bounding surface for this compartment.
+        point : List[float]
+            An interior-defining point for this compartment.
+        """
+        self.name = name
+        self.srfname = surface.name if isinstance(surface, Surface) else surface
+        self.point = point
+        self.simulation = simulation
+        assert self.point, "At least one point is required."
+        k = self.simulation.addCompartment(self.name)
+        assert k == _smoldyn.ErrorCode.ok
+        k = self.simulation.addCompartmentSurface(self.name, self.srfname)
+        assert k == _smoldyn.ErrorCode.ok
+        k = self.simulation.addCompartmentPoint(self.name, self.point)
+        assert k == _smoldyn.ErrorCode.ok
+
+    def addMolecules(self, species: Species, N: int):
+        """Place number of molecules in a compartment (uniformly distributed).
+
+        Parameters
+        ----------
+        N : int
+            number of molecules
+        species : Species
+            Species to add
+
+        See also
+        --------
+        :py:class:`smoldyn.kinetics.Species.addToCompartment`
+        """
+        assert N > 0, "Needs a positive number"
+        k = self.simulation.addCompartmentMolecules(species.name, N, self.name)
+        assert k == _smoldyn.ErrorCode.ok
+
+
+class Reaction(object):
+    __methoddict__ = dict(
+        i="irrev",
+        p="pgem",
+        x="pgemmax",
+        y="pgemmax2",
+        r="ratio",
+        b="unbindrad",
+        q="pgem2",
+        s="ratio2",
+        o="offset",
+        f="fixed",
+    )
+
+    def __init__(
+        self,
+        simulation: _smoldyn.Simulation,
+        name: str,
+        subs: List[SpeciesWithState],
+        prds: List[SpeciesWithState],
+        *,
+        rate: float = 0.0,
+        compartment: Compartment = None,
+        surface: Surface = None,
+        binding_radius: float = 0.0,
+        reaction_probability: float = 0.0,
+    ):
+        """Reaction (only occurs in forwared direction).
+
+        Parameters
+        ----------
+        simulation: _smoldyn.Simulation
+            Simulation object
+        name: str
+            name of the reaction.
+        subs : List[SpeciesWithState]
+            List of rectants.
+        prds : List[SpeciesWithState]
+            List of products.
+        rate : float
+            rate of the reaction
+        compartment: Compartment
+            If not ``None``, restrict the reaction to this compartment.
+        surface: Surface
+            If not ``None``, restricts this reaction to this surface.
+        binding_radius: float
+            binding radius (for second order reactions, if kf is not given)
+        reaction_probability: float
+            reaction probability (for first order reactions, if kf if not
+            given)
+        """
+        self.simulation = simulation
+        self.name = "r%d" % id(self) if not name else name
+        self.__rate = 0.0
+        self.subs = subs
+        self.prds = prds
+        self.reaction_probability = reaction_probability
+        self.binding_radius = binding_radius
+        self.compartment = compartment
+        self.surface = surface
+
+        assert len(subs) < 3, "At most two reactants are supported."
+        if subs is None or len(subs) == 0:
+            assert len(prds) > 0, "At least one product for a zero-order reaction."
+            subs = [NullSpecies()]
+        r1 = subs[0]
+        r2 = subs[1] if len(subs) == 2 else NullSpecies()
+
+        if isinstance(r1, Species):
+            r1name, r1state = r1.name, _toMS(r1.state)
+        else:
+            assert len(r1) == 2, "Expected tuple of (Species, state) e.g. (A, 'front')"
+            r1name = r1[0].name
+            r1state = _toMS(r1[1])
+
+        if isinstance(r2, Species):
+            r2name, r2state = r2.name, _toMS(r2.state)
+        else:
+            assert len(r2) == 2, "Expected tuple of (Species,state) e.g. (S, 'back')"
+            r2name, r2state = r2[0].name, _toMS(r2[1])
+
+        prdNames, prdStates = [], []
+        for x in prds:
+            if isinstance(x, Species):
+                prdNames.append(x.name)
+                prdStates.append(_toMS(x.state))
+            else:
+                prdNames.append(x[0].name)
+                prdStates.append(_toMS(x[1]))
+
+        k = self.simulation.addReaction(
+            name,
+            r1name,
+            r1state,
+            r2name,
+            r2state,
+            prdNames,
+            prdStates,
+            rate,
+        )
+        if k != _smoldyn.ErrorCode.ok:
+            __logger__.warning(f" Substrates: {subs}")
+            __logger__.warning(f" Products: {prds}, {prdNames}/{prdStates}")
+            raise RuntimeError(f"Failed to add reaction, ErrorCode {k}")
+
+        self.setRate(rate, reaction_probability, binding_radius)
+        if self.compartment is not None or self.surface is not None:
+            cname = self.compartment.name if self.compartment else ""
+            sname = self.surface.name if self.surface else ""
+            assert cname or sname
+            k = self.simulation.setReactionRegion(self.name, cname, sname)
+            assert k == _smoldyn.ErrorCode.ok
+
+    @property
+    def rate(self):
+        return self.__rate
+
+    @rate.setter
+    def rate(self, rate: float):
+        if rate != self.__rate:
+            self.__rate = rate
+            self.setRate(rate)
+
+    def setRate(self, rate, reaction_probability=-1.0, binding_radius=-1.0):
+        # if rate is negative, then we expect either binding_radius or
+        # reaction_probability. A reaction can have zero rate.
+        if rate >= 0.0:
+            k = self.simulation.setReactionRate(self.name, rate, False)
+            assert k == _smoldyn.ErrorCode.ok
+            return
+        elif rate < 0.0:
+            # check if reaction_probability is given
+            if len(self.subs) < 2:
+                assert (
+                    reaction_probability >= 0.0
+                ), "Must set rate or reaction_probability"
+                k = self.simulation.setReactionRate(
+                    self.name, reaction_probability, True
+                )
+                assert k == _smoldyn.ErrorCode.ok
+            else:
+                if reaction_probability >= 0.0:
+                    k = self.simulation.setReactionRate(self.name, reaction_probability, 2)
+                    assert k == _smoldyn.ErrorCode.ok
+                if binding_radius >= 0.0:
+                    k = self.simulation.setReactionRate(self.name, binding_radius, True)
+                    assert k == _smoldyn.ErrorCode.ok
+        else:
+            raise RuntimeError(
+                "Rate is not a numeric value"
+            )
+
+    @property
+    def order(self):
+        return len(self.subs)
+
+    def setIntersurface(self, rules: List[Union[int, str]]):
+        """Define `rules` to allow a bimolecular reaction operates when its
+        reactants are on different surfaces. In general, there should be as
+        many rule values as there are products for this reaction
+
+        Parameters
+        ----------
+        rules :
+            List of integer or string. For each product choose `1` (or
+            ``"r1"``) if it should be placed on the first reactant’s surface or
+            relative to that surface, and `2` (``"r2"``) if it should be placed
+            on the second reactant’s surface or relative to that surface. To
+            turn off intersurface reactions, which is the default behavior,
+            give rule_list as ``[-1]`` or ``None``.  To turn on intersurface
+            reactions for reactions that have no products, give rule_list as
+            ``[0]`` or ``[]``. This statement cannot be used together with the
+            ``setSerialNum`` function for the same reaction.
+
+        """
+        assert self.order == 2, "Bimoleculear reaction is needed."
+        assert len(rules) == len(
+            self.prds
+        ), "Length of rules should be equal to number of products"
+        rules = [-1] if rules is None else rules
+        rules = [0] if rules == [] else rules
+        _rules: List[int] = []
+
+        # r1, r2 are turned to 1, 2 etc.
+        for r in rules:
+            r = int(r[1:]) if isinstance(r, str) else int(r)
+            _rules.append(r)
+        k = self.simulation.setReactionIntersurface(self.name, _rules)
+        assert k == _smoldyn.ErrorCode.ok
+
+    def productPlacement(
+        self,
+        method: str,
+        param: float = 0.0,
+        product: str = "",
+        pos: List[float] = [],
+    ):
+        """Placement method and parameters for the products of reaction.
+        This also affects the binding radius of the reverse reaction, as
+        explained in the manual.
+
+        Parameters
+        ----------
+        method : 'irrev' ('i'), 'pgem' ('p'), 'pgemmax' ('x')
+            , 'pgemmax2' ('y'), 'ratio' ('r'), 'unbindrad' ('b')
+            , 'pgem2' ('q'), 'ratio2' ('s'), 'offset' ('o'), 'fixed' ('f')
+        param : float
+            Parameter value. Usually required except for type 'irrev'
+        product: str, optional
+            Required for type 'fixed' and 'offset'
+        pos:
+            Required for type 'fixed' and 'offset'
+
+        Notes
+        -----
+        To create a “bounce” type reaction, for simulating excluded volume,
+        enter the type as bounce.  In this case, enterno parameter for the
+        default algorithm orone parameter.The default algorithm, also entered
+        with a -2 parameter, performs ballistic reflection for spherical
+        molecules. Enter a parameter of -1 for an algorithm in which the reactant
+        edges get separated by the same amount as they used to overlap, along
+        their separation vector (e.g. consider two reactants each of radius 1,
+        so the binding radius is set to 2; then, if the center-to-center
+        distance is found to be 1.6, the molecules get separated to make the
+        center-to-center distance equal to 2.4).  Alternatively, you can use
+        the parameter value to define the new separation, which should be
+        larger than the binding radius.
+        """
+        method = self.__methoddict__.get(method, method)
+        revType = _smoldyn.RevParam.__members__[method]
+
+        if method in ["fixed", "offset"]:
+            assert product, "Product is required"
+            assert pos, "pos is required"
+        k = self.simulation.setReactionProducts(self.name, revType, param, product, pos)
+        assert k == _smoldyn.ErrorCode.ok
+
+
+class BidirectionalReaction(object):
+    def __init__(
+        self,
+        simulation: _smoldyn.Simulation,
+        name: str,
+        subs: List[SpeciesWithState],
+        prds: List[SpeciesWithState],
+        kf: float,
+        kb: float = 0.0,
+        *,
+        binding_radius: float = 0.0,
+        reaction_probability: float = 0.0,
+        compartment: Compartment = None,
+        surface: Surface = None,
+    ):
+        """A bidirectional chemical reaction that consists of two Reactions,
+        forward  (always present) and reverse (`None` if ``kb<=0.0``).
+
+        Parameters
+        ----------
+        simulation: _smoldyn.Simulation
+            Simulation object
+        name : str
+            name of the reaction.
+        subs : List[SpeciesWithState]
+            subtrates
+        prds : List[SpeciesWithState]
+            products
+        kf : float
+            Forward rate constant
+        kb : float
+            Backward rate constant (default 0.0)
+        binding_radius: float
+            Binding radius (for second order reaction)
+        reaction_probability: float
+            Reaction probability (first order reaction)
+        compartment : Compartment
+            Reaction compartment. If not `None`, both forward and reverse
+            reactions will be limited to this compartment.
+        surface : Surface
+            Reaction surface. If not `None`, both forward and reverse
+            reactions will be limited to this surface.
+        """
+        self.simulation = simulation
+        self.name = f"r{id(self):d}" if not name else name
+        fwdname, revname = (name + "fwd", name + "rev") if kb > 0.0 else (name, "")
+        self._kf = kf
+        self._kb = kb
+        self.forward = Reaction(
+            self.simulation,
+            fwdname,
+            subs,
+            prds,
+            rate=kf,
+            compartment=compartment,
+            surface=surface,
+            binding_radius=binding_radius,
+            reaction_probability=reaction_probability,
+        )
+
+        self.reverse = None
+        if self._kb > 0.0:
+            self.reverse = Reaction(
+                self.simulation,
+                revname,
+                prds,
+                subs,
+                rate=self._kb,
+                compartment=compartment,
+                surface=surface,
+            )
+
+    @property
+    def kf(self):
+        return self._kf
+
+    @kf.setter
+    def kf(self, val: float):
+        self.forward.setRate(val)
+
+    @property
+    def kb(self):
+        return self._kh
+
+    @kb.setter
+    def kb(self, val: float):
+        assert self.reverse
+        self.reverse.setRate(val)
+
+
+@dataclass
+class Partition(object):
+    simulation: _smoldyn.Simulation
+    name: str
+    value: float
+
+    def __post_init__(self):
+        """Sets the virtual partitions in the simulation volumne. Two
+        specialization is avaiable: :py:class:`MoleculePerBox`, and
+        :py:class:`Box`.
+
+        See also
+        --------
+        :py:class:`MoleculePerBox`
+        :py:class:`Box`
+        """
+        k = self.simulation.setPartitions(self.name, self.value)
+        assert k == _smoldyn.ErrorCode.ok, f"Failed to set partition: {k}"
+
+
+class MoleculePerBox(Partition):
+    def __init__(self, simulation: _smoldyn.Simulation, size: float):
+        warnings.warn(
+            "MoleculePerBox is deprecated. Please use setPartitions in the future",
+            DeprecationWarning,
+        )
+        super().__init__(simulation, "molperbox", size)
+
+
+class Box(Partition):
+    def __init__(self, simulation: _smoldyn.Simulation, size):
+        warnings.warn(
+            "Box is deprecated. Please use setPartitions in the future",
+            DeprecationWarning,
+        )
+        super().__init__(simulation, "boxsize", size)
+
+
+def addMoleculesToSolution(molecule, *args, **kwargs):
+    """Add molecules to the solution.
+
+    An alias of Species.addToSolution
+
+    See also
+    --------
+    Species.addToSolution
+    """
+    molecule.addMoleculesToSolution(*args, **kwargs)
+
+
+class Simulation(_smoldyn.Simulation):
+    """Simulation class. A :class:`Simulation` object is an unit of simulation.
+    it is recommended to create a :class:`Simulation` object for every standalone
+    model.
+
+    Note
+    ----
+
+    Every model starts with a Simulation object which has its unique
+    :class:`simstruct`. Note that a user can create as many arbitrary smoldyn
+    objects as one likes but these objects become active only when they
+    are added to a :class:`Simulation` object.
+
+    See also
+    --------
+
+    :class:`_smoldyn.Simulation`
+
+    """
+
+    def __init__(
+        self,
+        low: List[float],
+        high: List[float],
+        *,
+        boundary_type: BoundType = "r",
+        log_level: int = 3,
+        **kwargs,
+    ):
+        """Simulation class is a container for a complete model. An object of
+        this class is a stand-alone self-contained model.
+
+        Parameters
+        ----------
+        low:
+            Lower bound.
+        high:
+            Higher bound.
+
+        log_level: int, default 3
+            set log level for default logger.
+            1: DEBUG, 2: INFO, 3: WARNING, 4: ERROR, 5: CRITICAL
+
+        Other Parameters
+        ----------------
+        stop: `float`
+            Simulation stop time
+        dt: `float`
+            Simulation dt
+        start : `float`
+            Simulation start time.
+        output_files :
+            Declare output files that can be used in addCommand string.
+        seed: `int`
+            Set the random seed for the simulation.
+
+        See also
+        --------
+        :py:_smoldyn.simptr
+        """
+
+        # https://stackoverflow.com/a/50886750/1805129
+        logging.getLogger(__name__).setLevel(10 * log_level)
+        for handler in __logger__.handlers:
+            handler.setLevel(10 * log_level)
+
+        __logger__.info(f"Setting logging level to {log_level}")
+
+        assert low, f"You must pass low bound, current value {low}"
+        assert high, f"You must pass high bound, current value {high}"
+        if isinstance(boundary_type, str):
+            if len(boundary_type) == 1:
+                assert len(low) == len(
+                    high
+                ), f"dimension mismatch {len(low)} != {len(high)}"
+                boundary_type = boundary_type * len(low)
+            boundary_type = list(boundary_type)
+
+        super().__init__(low, high, boundary_type)
+
+        assert self.simptr, "Fatal error: Could not create simstruct"
+
+        # set filepath and filename at simptr
+        if __top_model_file__:
+            __top_model_file__.resolve()
+            super().setModelpath(str(__top_model_file__))
+
+        assert self.simptr, "Configuration is not initialized"
+        if kwargs.get("accuracy", 0.0):
+            self.accuracy: float = kwargs["accuracy"]
+
+        self.setOutputFiles(kwargs.get("output_files", []))
+
+        if kwargs.get("seed", -1) >= 0:
+            self.randomSeed = int(kwargs["seed"])
+
+#        if kwargs.get("log_level", 2):#????
+#            self.flags = kwargs["log_level"]	# Doesn't work
+
+    @classmethod
+    def fromFile(cls, path: Union[Path, str], arg: str = ""):
+        """Create `_smoldyn.Simulation` object from model file.
+
+        Parameters
+        ----------
+        path : T.Union[Path, str]
+            path
+        arg : str
+            arg
+        """
+        #  return _smoldyn.Simulation(str(path), arg)
+        obj = cls.__new__(cls)
+        path = Path(path).resolve()  # critical.
+        super(Simulation, obj).__init__(str(path), arg)
+        return obj
+
+    def setOutputFiles(self, outfiles: List[str], append=True):
+        """Declaration of filenames that can be used for output of simulation
+        results.  Spaces are not permitted in these names.  Any previous files
+        with the same name will be overwritten.
+
+        Parameters
+        ----------
+        outfiles : List[str]
+            Output files.  If all files don't have the same parent directory,
+            last file's parent directory is used.
+        append : bool
+            If `True`, append the data to the exsiting file. Default `False`.
+
+        See also
+        --------
+        setOutputFile
+        """
+        assert isinstance(outfiles, (list, tuple)), "Expecting a list of files"
+        for outfile in outfiles:
+            self.setOutputFile(outfile, append)
+
+    def setOutputFile(self, outfile, append: bool = False):
+        """Declaration of filenames that can be used for output of simulation
+        results.  Spaces are not permitted in these names.  Any previous files
+        with the same name will be overwritten.
+
+        Parameters
+        ----------
+        outfile : Union[str, Path]
+            Output file.
+        append : bool
+            If `True`, append the data to the exsiting file. Default `False`.
+
+        See also
+        --------
+        setOutputFiles
+        """
+        outfile = Path(outfile).resolve()
+        if outfile.parent != Path("."):
+            super().setOutputPath(str(outfile.parent) + "/")
+        # FIXME: Not sure what to do with second arg here.
+        super().addOutputFile(outfile.name, 0, append)
+
+    def setGraphics(
+        self,
+        method: str,
+        iter: int = 20,
+        delay: int = 0,
+        bg_color: ColorType = "white",
+        frame_thickness: int = 2,
+        frame_color: ColorType = "black",
+        grid_thickness: int = 0,
+        grid_color: ColorType = "white",
+        text_display: Union[List, str] = "",
+    ):
+        """Set graphics parameters for this simulation.
+
+        Parameters
+        ----------
+        method : str
+            Avaibale options: "none", "opengl", "opengl_good", "opengl_better"
+        iter : int
+            Update graphics after every nth step (default 20)
+        delay : int
+            Additional delay between rendering
+        bg_color: Color
+            Background color
+        frame_thickness: int
+            Thickness of the frame that is drawn around the simulation volume,
+            in pts. Default value is 2.
+        frame_color: Color
+            Specify the color of the frame. Default value is 'black'
+        grid_thickness: int
+            Thickness of the grid lines that can be drawn to show the virtual
+            boxes. Default value is 0, so that thegrid is not drawn.
+        grid_color: Color
+            Color of the grid. Default "white" or [1,1,1,1]
+        text_display:
+            List of variables to be displayed. Or a text string containing
+            variable names e.g. 'time E S ES(front)'
+        """
+        k = super().setGraphicsParams(method, iter, delay)
+        assert k == _smoldyn.ErrorCode.ok
+        k = super().setBackgroundStyle(Color(bg_color).rgba)
+        assert k == _smoldyn.ErrorCode.ok
+        k = super().setFrameStyle(frame_thickness, Color(frame_color).rgba)
+        assert k == _smoldyn.ErrorCode.ok
+
+        if grid_thickness > 0 and grid_color != bg_color:
+            k = super().setGridStyle(grid_thickness, Color(grid_color).rgba)
+            assert k == _smoldyn.ErrorCode.ok
+
+        self.setText(text_display)
+
+    # alias for setGraphics
+    addGraphics = setGraphics
+
+    @classmethod
+    def __todisp_text__(self, x):
+        if isinstance(x, str):
+            return x
+        if isinstance(x, tuple):
+            return f"{x[0].name}({x[1]})"
+        return x.__to_disp__()
+
+    def setText(self, text_display, color: ColorType = "black"):
+        if isinstance(text_display, str):
+            text_display = text_display.strip().split(" ")
+        for item in text_display:
+            if not item:
+                continue
+            k = super().addTextDisplay(self.__todisp_text__(item))
+            assert k == _smoldyn.ErrorCode.ok, f"Failed to set '{item}'"
+
+        k = super().setTextStyle(Color(color).rgba)
+        assert k == _smoldyn.ErrorCode.ok, "Failed to set text color"
+
+    def setTiff(
+        self,
+        tiffname: str = "OpenGL",
+        minsuffix: int = 1,
+        maxsuffix: int = 999,
+        every: int = 5,
+    ):
+        """TIFF related parameters.
+
+        Parameters
+        ----------
+        tiffname : str
+            Root filename for TIFF files, which may include path information if
+            desired. Default is “OpenGL”, which leads to the first TIFF being saved as
+            “OpenGL001.tif”.
+        minsuffix : int
+            Initial suffix number of TIFF files that are saved.  Default value
+            is 1.
+        maxsuffix : int
+            Largest possible suffix number of TIFF files that are saved.  Once
+            this value has been reached, additional TIFFs cannot be saved.
+            Default value is 999.
+        every: int
+            ``every`` is the number of simulation timesteps that should elapse
+            between subsequent snapshots.
+        """
+        k = super().setTiffParams(every, str(tiffname), minsuffix, maxsuffix)
+        assert k == _smoldyn.ErrorCode.ok
+
+    def setLight(
+        self,
+        index: int,
+        ambient: Color,
+        diffuse: Color,
+        specular: Color,
+        pos: List[float],
+    ):
+        """Set the parameters for a light source, for use with opengl_better
+        quality graphics. Parameters “ambient”, “diffuse”, “specular” are for
+        the light’s colors, which are then specified with either a word or in
+        the values as red, green, blue, and optionally alpha.
+
+        Parameters
+        ----------
+        index : int
+            The light index should be between 0 and 7.
+        ambient : Color
+            ambient
+        diffuse : Color
+            diffuse
+        specular : Color
+            specular
+        pos : List[float]
+            Light’s 3-dimensional position, which is specified as x, y,and zin
+            the values. Lights specified this way are automatically enabled
+            (turned on).
+        """
+        ambient = Color(ambient).rgba
+        diffuse = Color(diffuse).rgba
+        specular = Color(specular).rgba
+        k = super().setLightParams(index, ambient, diffuse, specular, pos)
+        assert k == _smoldyn.ErrorCode.ok
+
+    def run(
+        self,
+        stop: float,
+        dt: float,
+        *,
+        start: float = 0.0,
+        display: bool = True,
+        overwrite: bool = False,
+        accuracy=None,
+        log_level: int = 3,
+        quit_at_end: bool = False,
+    ):
+        """run the simulation.
+
+        Parameters
+        ----------
+        stop :
+            stop time
+        dt :
+            dt
+        start :
+            start (default 0.0)
+        accuracy :
+            accuracy
+        overwrite:
+            Overwrite existing data files.
+        display:
+            Show graphics (default True)
+        quit_at_end:
+            When set to `True`, smoldyn won't ask for Shift+Q at the end of simulation
+            to close the OpenGL window. Same effect can be achieved by setting
+            the environment variable SMOLDYN_NO_PROMPT. It is useful for
+            running tests in batch mode.
+        """
+
+        self.stop = float(stop)
+        self.dt = float(dt)
+        self.start = float(start)
+        if accuracy is not None:
+            self.accuracy = float(accuracy)
+
+        super().setSimTimes(self.start, self.stop, self.dt)
+
+        self.quitatend = quit_at_end
+
+        assert self.dt > 0.0, f"dt can't be <= 0.0! dt={self.dt}"
+        assert self.stop > 0.0, f"stop time can't be <= 0.0! stop={self.stop}"
+
+        k = super().runSim(self.stop, self.dt, display, overwrite)
+        assert _smoldyn.ErrorCode.ok == k, f"Expected ErrorCode.ok, got {k}"
+
+    def runUntil(self, stop, dt, display: bool = True, overwrite: bool = False):
+        """Run simulation until a given time.
+
+        Parameters
+        ----------
+        stop :
+            stop
+        dt :
+            dt
+
+        display : bool
+            Enable gui display (default `True`)?
+
+        overwrite : bool
+            Overwrite existing data (default `False`)?
+        """
+        self.stop = stop
+        self.dt = float(dt)
+
+        assert self.dt > 0.0, f"dt can't be <= 0.0! dt={self.dt}"
+        assert self.stop > 0.0, f"stop time can't be <= 0.0! stop={self.stop}"
+        super().runUntil(self.stop, self.dt, display, overwrite)
+
+    def updateSim(self):
+        """updateSim"""
+        super().updateSim()
+
+    def display(self):
+        k = super().displaySim()
+        assert k == _smoldyn.ErrorCode.ok
+
+    def addCommand(self, cmd: str, cmd_type: str, **kwargs):
+        """Add command.
+
+        Parameters
+        ----------
+        cmd: str
+            Command string.
+
+        cmd_type: str
+            Type of command. Optional when `from_string` is set to `True`. Then
+            the type is to be included in the `cmd` string itself.
+
+            Use capital letter version for integer queue.  ‘b’ or 'B' for
+            before the simulation.  ‘a’ or 'A' for after the simulation.  ‘e’
+            or 'E' for every time step during the simulation.  ‘@’ or '&' for a
+            single command execution at time `time`.  ‘n’ or 'N' for every n’th
+            iteration of the simulation.  ‘i’ or 'I' for a fixed time interval.
+            The command is executed over the period from on to off with
+            intervals of at least dt (the actual intervals will only end at the
+            times of simulation time steps).  ‘x’ for a fixed time multiplier.
+            The command is executed at on, then on+dt, then on+dt*xt, then
+            on+dt*xt2, and so forth.  ‘j’ for every ``dtit`` step with a set
+            starting iteration and stopping iteration.
+
+        kwargs: dict
+            kwargs of :func:`_smoldyn.Command()`.
+
+        """
+        if "step" not in kwargs:
+            kwargs["step"] = self.dt
+        super().addCommand(cmd, cmd_type[0], **kwargs)
+
+    def addCommandStr(self, cmd: str):
+        """Add command using a single string. See the Smoldyn's User Manual for
+        details.
+
+        Parameters
+        ----------
+        cmd : str
+            Command string
+        """
+        super().addCommandStr(cmd)
+
+    # mapping.
+    def addSpecies(
+        self,
+        name: str,
+        state: str = "soln",
+        color: Union[ColorType, Dict[str, ColorType]] = {"soln": "black"},
+        difc: Union[float, Dict[str, float]] = 0.0,
+        display_size: float = 3,
+        mol_list: str = "",
+    ) -> Species:
+        """Add species to Simulation
+
+        See :class:`smoldyn.Species` docs.
+        """
+        # Create a species.
+        s = Species(super(), name, state, color, difc, display_size, mol_list)
+        return s
+
+    def addMolecules(
+        self,
+        species: Species,
+        number: int,
+        pos: List[float] = [],
+        lowpos: List[float] = [],
+        highpos: List[float] = [],
+    ):
+        """See :func:`Species.addToSolution`"""
+        species.addToSolution(number, pos, lowpos, highpos)
+
+    def addSurface(self, name: str, *, panels: List[Panel]) -> Surface:
+        """See :class:`Surface` docs"""
+        return Surface(simulation=super(), name=name, panels=panels)
+
+    def addBidirectionalReaction(
+        self,
+        name: str,
+        subs: List[SpeciesWithState],
+        prds: List[SpeciesWithState],
+        kf: float,
+        kb: float = 0.0,
+        *,
+        binding_radius: float = 0.0,
+        reaction_probability: float = 0.0,
+        compartment: Compartment = None,
+        surface: Surface = None,
+    ) -> BidirectionalReaction:
+
+        return BidirectionalReaction(
+            super(),
+            name,
+            subs,
+            prds,
+            kf,
+            kb,
+            binding_radius=binding_radius,
+            reaction_probability=reaction_probability,
+            compartment=compartment,
+            surface=surface,
+        )
+
+    def addReaction(
+        self,
+        name: str,
+        subs: List[SpeciesWithState],
+        prds: List[SpeciesWithState],
+        *,
+        rate: float = 0.0,
+        compartment: Compartment = None,
+        surface: Surface = None,
+        binding_radius: float = 0.0,
+        reaction_probability: float = 0.0,
+    ) -> Reaction:
+        """Add a reaction (unidirectional)
+
+        See Reaction for details.
+        """
+        return Reaction(
+            super(),
+            name,
+            subs,
+            prds,
+            rate=rate,
+            compartment=compartment,
+            surface=surface,
+            binding_radius=binding_radius,
+            reaction_probability=reaction_probability,
+        )
+
+    def addPartition(self, name: str, value):
+        """Sets the virtual partitions in the simulation volumne. Two
+        specialization is avaiable: :py:class:`MoleculePerBox`, and
+        :py:class:`Box`.
+
+        See also
+        --------
+        :py:class:`MoleculePerBox`
+        :py:class:`Box`
+        """
+        return Partition(super(), name, value)
+
+    def addBox(self, size: float):
+        """See Box.__init__"""
+
+        warnings.warn(
+            "This function is deprecated. Please use setPartitions in the future",
+            DeprecationWarning,
+        )
+        return Box(super(), size)
+
+    def addMoleculePerBox(self, size: float):
+        """See MoleculePerBox.__init__"""
+
+        warnings.warn(
+            "This function is deprecated. Please use setPartitions in the future",
+            DeprecationWarning,
+        )
+        return MoleculePerBox(super(), size)
+
+    def addCompartment(
+        self, name: str, *, surface: Union[str, Surface], point: List[float]
+    ):
+        return Compartment(super(), name, surface=surface, point=point)
+
+    def addOutputData(self, dataname: str) -> None:
+        """Declares the data table called `dataname`, enabling output into it by
+        one or more runtime commands. Spaces are not permitted in the dataname.
+
+        Parameters
+        ----------
+        dataname : str
+            dataname (spaces are not allowed)
+
+        Returns
+        -------
+        None
+
+        """
+        assert " " not in dataname, f"spaces not allowed in dataname: '{dataname}'"
+        r = super().addOutputData(dataname)
+        assert r == _smoldyn.ErrorCode.ok, f"Failed to add output data {r}"
+
+    def getOutputData(self, dataname: str, erase: bool = True) -> List[List[float]]:
+        """Returns data that have been recorded by an observation command (e.g. molcount).
+
+        Parameters
+        ----------
+        dataname : str
+            dataname
+
+        erase: bool
+            When set to `True`, the original data is cleared after a copy  of data
+            is returned to the user.
+
+        Returns
+        -------
+        List[List[float]]
+            A matrix of float.
+        """
+        assert " " not in dataname, f"Must not contain spaces: '{dataname}'"
+        y: List[List[float]] = super().getOutputData(dataname, erase)
+        return y
+
+    def connect(self, func, target, step: int, args: List[float] = []):
+        """Connect a arbitrary Python function to Simulation. The function will
+        be called at every 'step'
+
+        Parameters
+        ----------
+        func :
+            Python function to connect. It must have two arguments. The first
+            argument is always simulation time 't'. the second argument is a
+            list of float which refers to `args` (4th argument of this function)
+        target :
+            Target function or a property. The return value of the connected function
+            i.e., func is the argument to this function.
+        step : int
+            The connected function func is called after these many simulation
+            steps.
+        args : List[float]
+            argument of func (passed by reference). Any change in this list will
+            be visible to func.
+
+        Example
+        -------
+
+        >>> import math
+        >>> s = smoldyn.Simulation(low=(0, 0), high=(10, 10))
+        >>> a = s.addSpecies("a", color="black", difc=0.1)
+        >>> avals = []
+
+        >>> def func(t, args):
+        >>>     global a, avals
+        >>>     x, y = args
+        >>>     avals.append((t, a.difc["soln"]))
+        >>>     return x * math.sin(t) + y
+
+        >>> def target(val):
+        >>>     global a
+        >>>     a.difc = val
+
+        >>> s.connect(func, target, step=10, args=[1, 1])
+        >>> s.run(100, dt=1)
+        >>> avals
+        [(1.0, 0.1),
+         (11.0, 1.8414709848078965),
+         (21.0, 9.793449296524592e-06),
+         (31.0, 1.836655638536056),
+         (41.0, 0.595962354676935),
+         (51.0, 0.841377331195291),
+         (61.0, 1.6702291758433747),
+         (71.0, 0.03388222999160706),
+         (81.0, 1.9510546532543747),
+         (91.0, 0.37011200572554614)]
+        """
+        return super().connect(func, target, step, args)
+
+    def addPath2D(self, *points, closed: bool = False):
+        return Path2D(*points, simulation=super(), closed=closed)
+
+    def addPort(
+        self,
+        *,
+        name: str,
+        surface: Union[Surface, str],
+        panel: str,
+    ):
+        return Port(super(), name=name, surface=surface, panel=panel)
+
+    def addPanel(
+        self,
+        *,
+        name: str = "",
+        shape: _smoldyn.PanelShape = _smoldyn.PanelShape.none,
+        neighbors: List = [],
+    ):
+        return Panel(name=name, shape=shape, neighbors=neighbors, simulation=super())
+
+    def addTriangle(self, *, vertices: Sequence[Sequence[float]] = [[]], name=""):
+        return Triangle(simulation=super(), vertices=vertices, name=name)
+
+    def addRectangle(
+        self,
+        corner: Sequence[float],
+        dimensions: Sequence[float],
+        axis: str,
+        name="",
+    ):
+        return Rectangle(
+            simulation=super(),
+            corner=corner,
+            dimensions=dimensions,
+            axis=axis,
+            name=name,
+        )
+
+    def addSphere(
+        self,
+        *,
+        center: List[float],
+        radius: float,
+        slices: int,
+        stacks: int = 0,
+        name="",
+    ):
+        return Sphere(
+            simulation=super(),
+            center=center,
+            radius=radius,
+            slices=slices,
+            stacks=stacks,
+            name=name,
+        )
+
+    def addHemisphere(
+        self,
+        *,
+        center: List[float],
+        radius: float,
+        vector: List[float],
+        slices: int,
+        stacks: int,
+        name: str = "",
+    ):
+        return Hemisphere(
+            simulation=super(),
+            center=center,
+            radius=radius,
+            vector=vector,
+            slices=slices,
+            stacks=stacks,
+            name=name,
+        )
+
+    def addCylinder(
+        self,
+        *,
+        start: List[float],
+        end: List[float],
+        radius: float,
+        slices: int,
+        stacks: int,
+        name: str = "",
+    ):
+        return Cylinder(
+            simulation=super(),
+            start=start,
+            end=end,
+            radius=radius,
+            slices=slices,
+            stacks=stacks,
+            name=name,
+        )
+
+    def addDisk(
+        self,
+        *,
+        center: List[float],
+        radius: float,
+        slices: int,
+        vector: List[float],
+        name="",
+    ):
+        return Disk(
+            simulation=super(),
+            center=center,
+            radius=radius,
+            slices=slices,
+            vector=vector,
+            name=name,
+        )
```

## smoldyn/__init__.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-"""smoldyn
-
-Python bindings of Smoldyn simulator..
-
-To access the developer API, use `import smoldyn._smoldyn` namespace.
-"""
-
-"""Bring symbols from User API (smoldyn.py) to top-level."""
-from smoldyn.smoldyn import *
+"""smoldyn
+
+Python bindings of Smoldyn simulator..
+
+To access the developer API, use `import smoldyn._smoldyn` namespace.
+"""
+
+"""Bring symbols from User API (smoldyn.py) to top-level."""
+from smoldyn.smoldyn import *
```

## smoldyn/types.py

 * *Ordering differences only*

```diff
@@ -1,38 +1,38 @@
-"""
-Types
-"""
-
-from typing import Union, Tuple, Dict, List
-from smoldyn.utils import color2RGBA
-
-# Either a string such as 'black', 'red', 'orange' or a tuple of 4 values such
-# as [1,1,0,1] specifying RGBA value.
-ColorType = Union[str, Tuple[float, float, float], Tuple[float, float, float, float]]
-
-"""Diffusion coefficient can be a single numerical value (applies to all states
-of molecules), or it could be a dictionary of molecule state and correponding
-diffusion coefficient. 
-"""
-DiffConst = Union[float, Dict[str, float]]
-
-"""Boundary type e.g. 'r' or 'rrr' or ['r', 'r', 'r']. If a single value is
-given, it applies to all dimentions."""
-BoundType = Union[str, List[str]]
-
-class Color:
-    """Color class.
-    """
-    def __init__(self, color):
-        assert not isinstance(color, dict)
-        self.name = color if not isinstance(color, Color) else color.name
-        self.rgba = self._toRGBA()
-
-    def _toRGBA(self):
-        if isinstance(self.name, str):
-            return color2RGBA(self.name) if self.name else None
-        if len(self.name) == 3:
-            return (*self.name, 1)
-
-    def __str__(self):
-        return str(self.name)
-
+"""
+Types
+"""
+
+from typing import Union, Tuple, Dict, List
+from smoldyn.utils import color2RGBA
+
+# Either a string such as 'black', 'red', 'orange' or a tuple of 4 values such
+# as [1,1,0,1] specifying RGBA value.
+ColorType = Union[str, Tuple[float, float, float], Tuple[float, float, float, float]]
+
+"""Diffusion coefficient can be a single numerical value (applies to all states
+of molecules), or it could be a dictionary of molecule state and correponding
+diffusion coefficient. 
+"""
+DiffConst = Union[float, Dict[str, float]]
+
+"""Boundary type e.g. 'r' or 'rrr' or ['r', 'r', 'r']. If a single value is
+given, it applies to all dimentions."""
+BoundType = Union[str, List[str]]
+
+class Color:
+    """Color class.
+    """
+    def __init__(self, color):
+        assert not isinstance(color, dict)
+        self.name = color if not isinstance(color, Color) else color.name
+        self.rgba = self._toRGBA()
+
+    def _toRGBA(self):
+        if isinstance(self.name, str):
+            return color2RGBA(self.name) if self.name else None
+        if len(self.name) == 3:
+            return (*self.name, 1)
+
+    def __str__(self):
+        return str(self.name)
+
```

## smoldyn/utils.py

 * *Ordering differences only*

```diff
@@ -1,43 +1,43 @@
-# -*- coding: utf-8 -*-
-
-__author__ = "Dilawar Singh"
-__copyright__ = "Copyright 2019-, Dilawar Singh"
-__maintainer__ = "Dilawar Singh"
-__email__ = "dilawars@ncbs.res.in"
-
-import smoldyn._smoldyn  # type: ignore
-import typing as T
-
-__matplotlib_found__ = False
-try:
-    from matplotlib import colors  # type: ignore
-
-    __matplotlib_found__ = True
-except ImportError:
-    __matplotlib_found__ = False
-
-
-def load_model(path, *args):
-    smoldyn._smoldyn.load_model(path, *args)
-
-
-def color2RGBA(colorname: str) -> T.Tuple[float, float, float, float]:
-    """Convert color name to RGBA value.
-
-    If `matplotlib` is installed, its `colors` submodule is used else in-built
-    color parser is used which has limited number of colors.
-
-    Parameters
-    ----------
-    colorname : str
-        Name of the color
-
-    Return:
-    ------
-        A tuple of 4 values between 0 and 1.0 (red, green, blue, alpha)
-    """
-    if __matplotlib_found__:
-        clr: T.Tuple[float, float, float, float] = colors.to_rgba(colorname)
-    else:
-        clr = smoldyn._smoldyn.color2RGBA(colorname)
-    return clr
+# -*- coding: utf-8 -*-
+
+__author__ = "Dilawar Singh"
+__copyright__ = "Copyright 2019-, Dilawar Singh"
+__maintainer__ = "Dilawar Singh"
+__email__ = "dilawars@ncbs.res.in"
+
+import smoldyn._smoldyn  # type: ignore
+import typing as T
+
+__matplotlib_found__ = False
+try:
+    from matplotlib import colors  # type: ignore
+
+    __matplotlib_found__ = True
+except ImportError:
+    __matplotlib_found__ = False
+
+
+def load_model(path, *args):
+    smoldyn._smoldyn.load_model(path, *args)
+
+
+def color2RGBA(colorname: str) -> T.Tuple[float, float, float, float]:
+    """Convert color name to RGBA value.
+
+    If `matplotlib` is installed, its `colors` submodule is used else in-built
+    color parser is used which has limited number of colors.
+
+    Parameters
+    ----------
+    colorname : str
+        Name of the color
+
+    Return:
+    ------
+        A tuple of 4 values between 0 and 1.0 (red, green, blue, alpha)
+    """
+    if __matplotlib_found__:
+        clr: T.Tuple[float, float, float, float] = colors.to_rgba(colorname)
+    else:
+        clr = smoldyn._smoldyn.color2RGBA(colorname)
+    return clr
```

## smoldyn/__main__.py

 * *Ordering differences only*

```diff
@@ -1,27 +1,27 @@
-# -*- coding: utf-8 -*-
-
-__author__ = "Dilawar Singh"
-__email__ = "dilawar.s.rajput@gmail.com"
-
-import smoldyn._smoldyn  # type: ignore
-import argparse
-
-
-def main():
-    # Argument parser.
-    description = """Command-line interface to Smoldyn."""
-    parser = argparse.ArgumentParser(description=description)
-    parser.add_argument("input", help="Input file")
-    parser.add_argument(
-        "--overwrite", "-w", action="store_true", help="Overwrite exsiting data file"
-    )
-    parser.add_argument("--quit-at-end", "-q", action="store_true", help="Quit at end")
-    parser.add_argument(
-        "--args", "-A", default="", type=str, help="smoldyn command line arguments"
-    )
-    args = parser.parse_args()
-    smoldyn._smoldyn.loadModel(args.input, args.args, args.overwrite, args.quit_at_end)
-
-
-if __name__ == "__main__":
-    main()
+# -*- coding: utf-8 -*-
+
+__author__ = "Dilawar Singh"
+__email__ = "dilawar.s.rajput@gmail.com"
+
+import smoldyn._smoldyn  # type: ignore
+import argparse
+
+
+def main():
+    # Argument parser.
+    description = """Command-line interface to Smoldyn."""
+    parser = argparse.ArgumentParser(description=description)
+    parser.add_argument("input", help="Input file")
+    parser.add_argument(
+        "--overwrite", "-w", action="store_true", help="Overwrite exsiting data file"
+    )
+    parser.add_argument("--quit-at-end", "-q", action="store_true", help="Quit at end")
+    parser.add_argument(
+        "--args", "-A", default="", type=str, help="smoldyn command line arguments"
+    )
+    args = parser.parse_args()
+    smoldyn._smoldyn.loadModel(args.input, args.args, args.overwrite, args.quit_at_end)
+
+
+if __name__ == "__main__":
+    main()
```

## smoldyn/biosimulators/combine.py

 * *Ordering differences only*

```diff
@@ -1,959 +1,959 @@
-''' Methods for executing COMBINE archives and SED-ML files involving simulations of models encoded in Smoldyn
-
-    Information about encoding Smoldyn simulations into SED-ML files and COMBINE archives is available at
-    `https://github.com/ssandrews/Smoldyn/blob/master/Using-Smoldyn-with-SED-ML-COMBINE-BioSimulators.md <https://github.com/ssandrews/Smoldyn/blob/master/Using-Smoldyn-with-SED-ML-COMBINE-BioSimulators.md>`_.
-'''
-
-__author__ = 'Jonathan Karr'
-__email__ = 'karr@mssm.edu'
-
-__all__ = [
-    'exec_sedml_docs_in_combine_archive',
-    'exec_sed_task',
-]
-
-from .data_model import (SmoldynCommand, SmoldynOutputFile, SimulationChange, SimulationChangeExecution, AlgorithmParameterType,
-                         KISAO_ALGORITHMS_MAP, KISAO_ALGORITHM_PARAMETERS_MAP)
-from biosimulators_utils.combine.exec import exec_sedml_docs_in_archive
-from biosimulators_utils.config import get_config, Config  # noqa: F401
-from biosimulators_utils.log.data_model import CombineArchiveLog, TaskLog, StandardOutputErrorCapturerLevel  # noqa: F401
-from biosimulators_utils.viz.data_model import VizFormat  # noqa: F401
-from biosimulators_utils.report.data_model import ReportFormat, VariableResults, SedDocumentResults  # noqa: F401
-from biosimulators_utils.sedml import validation
-from biosimulators_utils.sedml.data_model import (Task, ModelLanguage, ModelAttributeChange,  # noqa: F401
-                                                  UniformTimeCourseSimulation, AlgorithmParameterChange, Variable,
-                                                  Symbol)
-from biosimulators_utils.sedml.exec import exec_sed_doc as base_exec_sed_doc
-from biosimulators_utils.utils.core import validate_str_value, parse_value, raise_errors_warnings
-from smoldyn import smoldyn
-import functools
-import os
-import numpy
-import pandas
-import re
-import tempfile
-import types  # noqa: F401
-
-__all__ = ['exec_sedml_docs_in_combine_archive', 'exec_sed_task', 'exec_sed_doc', 'preprocess_sed_task']
-
-
-def exec_sedml_docs_in_combine_archive(archive_filename, out_dir, config=None):
-    ''' Execute the SED tasks defined in a COMBINE/OMEX archive and save the outputs
-
-    Args:
-        archive_filename (:obj:`str`): path to COMBINE/OMEX archive
-        out_dir (:obj:`str`): path to store the outputs of the archive
-
-            * CSV: directory in which to save outputs to files
-              ``{ out_dir }/{ relative-path-to-SED-ML-file-within-archive }/{ report.id }.csv``
-            * HDF5: directory in which to save a single HDF5 file (``{ out_dir }/reports.h5``),
-              with reports at keys ``{ relative-path-to-SED-ML-file-within-archive }/{ report.id }`` within the HDF5 file
-
-        config (:obj:`Config`, optional): BioSimulators common configuration
-
-    Returns:
-        :obj:`tuple`:
-
-            * :obj:`SedDocumentResults`: results
-            * :obj:`CombineArchiveLog`: log
-    '''
-    return exec_sedml_docs_in_archive(exec_sed_doc, archive_filename, out_dir,
-                                      apply_xml_model_changes=False,
-                                      config=config)
-
-
-def exec_sed_doc(doc, working_dir, base_out_path, rel_out_path=None,
-                 apply_xml_model_changes=True,
-                 log=None, indent=0, pretty_print_modified_xml_models=False,
-                 log_level=StandardOutputErrorCapturerLevel.c, config=None):
-    """ Execute the tasks specified in a SED document and generate the specified outputs
-
-    Args:
-        doc (:obj:`SedDocument` or :obj:`str`): SED document or a path to SED-ML file which defines a SED document
-        working_dir (:obj:`str`): working directory of the SED document (path relative to which models are located)
-
-        base_out_path (:obj:`str`): path to store the outputs
-
-            * CSV: directory in which to save outputs to files
-              ``{base_out_path}/{rel_out_path}/{report.id}.csv``
-            * HDF5: directory in which to save a single HDF5 file (``{base_out_path}/reports.h5``),
-              with reports at keys ``{rel_out_path}/{report.id}`` within the HDF5 file
-
-        rel_out_path (:obj:`str`, optional): path relative to :obj:`base_out_path` to store the outputs
-        apply_xml_model_changes (:obj:`bool`, optional): if :obj:`True`, apply any model changes specified in the SED-ML file before
-            calling :obj:`task_executer`.
-        log (:obj:`SedDocumentLog`, optional): log of the document
-        indent (:obj:`int`, optional): degree to indent status messages
-        pretty_print_modified_xml_models (:obj:`bool`, optional): if :obj:`True`, pretty print modified XML models
-        log_level (:obj:`StandardOutputErrorCapturerLevel`, optional): level at which to log output
-        config (:obj:`Config`, optional): BioSimulators common configuration
-        simulator_config (:obj:`SimulatorConfig`, optional): tellurium configuration
-
-    Returns:
-        :obj:`tuple`:
-
-            * :obj:`ReportResults`: results of each report
-            * :obj:`SedDocumentLog`: log of the document
-    """
-    return base_exec_sed_doc(exec_sed_task, doc, working_dir, base_out_path,
-                             rel_out_path=rel_out_path,
-                             apply_xml_model_changes=apply_xml_model_changes,
-                             log=log,
-                             indent=indent,
-                             pretty_print_modified_xml_models=pretty_print_modified_xml_models,
-                             log_level=log_level,
-                             config=config)
-
-
-def exec_sed_task(task, variables, preprocessed_task=None, log=None, config=None):
-    ''' Execute a task and save its results
-
-    Args:
-       task (:obj:`Task`): task
-       variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
-       preprocessed_task (:obj:`dict`, optional): preprocessed information about the task, including possible
-            model changes and variables. This can be used to avoid repeatedly executing the same initialization
-            for repeated calls to this method.
-       log (:obj:`TaskLog`, optional): log for the task
-       config (:obj:`Config`, optional): BioSimulators common configuration
-
-    Returns:
-        :obj:`tuple`:
-
-            :obj:`VariableResults`: results of variables
-            :obj:`TaskLog`: log
-    '''
-    if not config:
-        config = get_config()
-
-    if config.LOG and not log:
-        log = TaskLog()
-
-    sed_model_changes = task.model.changes
-    sed_simulation = task.simulation
-
-    if preprocessed_task is None:
-        preprocessed_task = preprocess_sed_task(task, variables, config=config)
-        sed_model_changes = list(filter(lambda change: change.target in preprocessed_task['sed_smoldyn_simulation_change_map'],
-                                        sed_model_changes))
-
-    # read Smoldyn configuration
-    smoldyn_simulation = preprocessed_task['simulation']
-
-    # apply model changes to the Smoldyn configuration
-    sed_smoldyn_simulation_change_map = preprocessed_task['sed_smoldyn_simulation_change_map']
-    for change in sed_model_changes:
-        smoldyn_change = sed_smoldyn_simulation_change_map.get(change.target, None)
-        if smoldyn_change is None or smoldyn_change.execution != SimulationChangeExecution.simulation:
-            raise NotImplementedError('Target `{}` can only be changed during simulation preprocessing.'.format(change.target))
-        apply_change_to_smoldyn_simulation(
-            smoldyn_simulation, change, smoldyn_change)
-
-    # get the Smoldyn representation of the SED uniform time course simulation
-    smoldyn_simulation_run_timecourse_args = get_smoldyn_run_timecourse_args(sed_simulation)
-
-    # execute the simulation
-    smoldyn_run_args = dict(
-        **smoldyn_simulation_run_timecourse_args,
-        **preprocessed_task['simulation_run_alg_param_args'],
-    )
-    smoldyn_simulation.run(**smoldyn_run_args, overwrite=True, display=False, quit_at_end=False)
-
-    # get the result of each SED variable
-    variable_output_cmd_map = preprocessed_task['variable_output_cmd_map']
-    smoldyn_output_files = preprocessed_task['output_files']
-    variable_results = get_variable_results(sed_simulation.number_of_steps, variables, variable_output_cmd_map, smoldyn_output_files)
-
-    # cleanup output files
-    for smoldyn_output_file in smoldyn_output_files.values():
-        os.remove(smoldyn_output_file.filename)
-
-    # log simulation
-    if config.LOG:
-        log.algorithm = sed_simulation.algorithm.kisao_id
-        log.simulator_details = {
-            'class': 'smoldyn.Simulation',
-            'instanceAttributes': preprocessed_task['simulation_attrs'],
-            'method': 'run',
-            'methodArguments': smoldyn_run_args,
-        }
-
-    # return the values of the variables and log
-    return variable_results, log
-
-
-def preprocess_sed_task(task, variables, config=None):
-    """ Preprocess a SED task, including its possible model changes and variables. This is useful for avoiding
-    repeatedly initializing tasks on repeated calls of :obj:`exec_sed_task`.
-
-    Args:
-        task (:obj:`Task`): task
-        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
-        config (:obj:`Config`, optional): BioSimulators common configuration
-
-    Returns:
-        :obj:`dict`: preprocessed information about the task
-    """
-    config = config or get_config()
-
-    sed_model = task.model
-    sed_simulation = task.simulation
-
-    if config.VALIDATE_SEDML:
-        raise_errors_warnings(validation.validate_task(task),
-                              error_summary='Task `{}` is invalid.'.format(task.id))
-        raise_errors_warnings(validation.validate_model_language(sed_model.language, ModelLanguage.Smoldyn),
-                              error_summary='Language for model `{}` is not supported.'.format(sed_model.id))
-        raise_errors_warnings(validation.validate_model_change_types(sed_model.changes, (ModelAttributeChange, )),
-                              error_summary='Changes for model `{}` are not supported.'.format(sed_model.id))
-        raise_errors_warnings(*validation.validate_model_changes(sed_model),
-                              error_summary='Changes for model `{}` are invalid.'.format(sed_model.id))
-        raise_errors_warnings(validation.validate_simulation_type(sed_simulation, (UniformTimeCourseSimulation, )),
-                              error_summary='{} `{}` is not supported.'.format(sed_simulation.__class__.__name__, sed_simulation.id))
-        raise_errors_warnings(*validation.validate_simulation(sed_simulation),
-                              error_summary='Simulation `{}` is invalid.'.format(sed_simulation.id))
-        raise_errors_warnings(*validation.validate_data_generator_variables(variables),
-                              error_summary='Data generator variables for task `{}` are invalid.'.format(task.id))
-
-    if sed_simulation.algorithm.kisao_id not in KISAO_ALGORITHMS_MAP:
-        msg = 'Algorithm `{}` is not supported. The following algorithms are supported:{}'.format(
-            sed_simulation.algorithm.kisao_id,
-            ''.join('\n  {}: {}'.format(kisao_id, alg_props['name']) for kisao_id, alg_props in KISAO_ALGORITHMS_MAP.items())
-        )
-        raise NotImplementedError(msg)
-
-    # read Smoldyn configuration
-    simulation_configuration = read_smoldyn_simulation_configuration(sed_model.source)
-    normalize_smoldyn_simulation_configuration(simulation_configuration)
-
-    # turn off Smoldyn's graphics
-    disable_smoldyn_graphics_in_simulation_configuration(simulation_configuration)
-
-    # preprocess model changes
-    sed_smoldyn_preprocessing_change_map = {}
-    sed_smoldyn_simulation_change_map = {}
-    for change in sed_model.changes:
-        smoldyn_change = validate_model_change(change)
-
-        if smoldyn_change.execution == SimulationChangeExecution.preprocessing:
-            sed_smoldyn_preprocessing_change_map[change] = smoldyn_change
-        else:
-            sed_smoldyn_simulation_change_map[change.target] = smoldyn_change
-
-    # apply preprocessing-time changes
-    for change, smoldyn_change in sed_smoldyn_preprocessing_change_map.items():
-        apply_change_to_smoldyn_simulation_configuration(
-            simulation_configuration, change, smoldyn_change)
-
-    # write the modified Smoldyn configuration to a temporary file
-    fid, smoldyn_configuration_filename = tempfile.mkstemp(suffix='.txt')
-    os.close(fid)
-    write_smoldyn_simulation_configuration(simulation_configuration, smoldyn_configuration_filename)
-
-    # initialize a simulation from the Smoldyn file
-    smoldyn_simulation = init_smoldyn_simulation_from_configuration_file(smoldyn_configuration_filename)
-
-    # clean up temporary file
-    os.remove(smoldyn_configuration_filename)
-
-    # apply the SED algorithm parameters to the Smoldyn simulation and to the arguments to its ``run`` method
-    smoldyn_simulation_attrs = {}
-    smoldyn_simulation_run_alg_param_args = {}
-    for sed_algorithm_parameter_change in sed_simulation.algorithm.changes:
-        val = get_smoldyn_instance_attr_or_run_algorithm_parameter_arg(sed_algorithm_parameter_change)
-        if val['type'] == AlgorithmParameterType.run_argument:
-            smoldyn_simulation_run_alg_param_args[val['name']] = val['value']
-        else:
-            smoldyn_simulation_attrs[val['name']] = val['value']
-
-    # apply the SED algorithm parameters to the Smoldyn simulation and to the arguments to its ``run`` method
-    for attr_name, value in smoldyn_simulation_attrs.items():
-        setter = getattr(smoldyn_simulation, attr_name)
-        setter(value)
-
-    # validate SED variables
-    variable_output_cmd_map = validate_variables(variables)
-
-    # Setup Smoldyn output files for the SED variables
-    smoldyn_configuration_dirname = os.path.dirname(smoldyn_configuration_filename)
-    smoldyn_output_files = add_smoldyn_output_files_for_sed_variables(
-        smoldyn_configuration_dirname, variables, variable_output_cmd_map, smoldyn_simulation)
-
-    # return preprocessed information
-    return {
-        'simulation': smoldyn_simulation,
-        'simulation_attrs': smoldyn_simulation_attrs,
-        'simulation_run_alg_param_args': smoldyn_simulation_run_alg_param_args,
-        'sed_smoldyn_simulation_change_map': sed_smoldyn_simulation_change_map,
-        'variable_output_cmd_map': variable_output_cmd_map,
-        'output_files': smoldyn_output_files,
-    }
-
-
-def init_smoldyn_simulation_from_configuration_file(filename):
-    ''' Initialize a simulation for a Smoldyn model from a file
-
-    Args:
-        filename (:obj:`str`): path to model file
-
-    Returns:
-        :obj:`smoldyn.Simulation`: simulation
-    '''
-    if not os.path.isfile(filename):
-        raise FileNotFoundError('Model source `{}` is not a file.'.format(filename))
-
-    smoldyn_simulation = smoldyn.Simulation.fromFile(filename)
-    if not smoldyn_simulation.getSimPtr():
-        error_code, error_msg = smoldyn.getError()
-        msg = 'Model source `{}` is not a valid Smoldyn file.\n\n  {}: {}'.format(
-            filename, error_code.name[0].upper() + error_code.name[1:], error_msg.replace('\n', '\n  '))
-        raise ValueError(msg)
-
-    return smoldyn_simulation
-
-
-def read_smoldyn_simulation_configuration(filename):
-    ''' Read a configuration for a Smoldyn simulation
-
-    Args:
-        filename (:obj:`str`): path to model file
-
-    Returns:
-        :obj:`list` of :obj:`str`: simulation configuration
-    '''
-    with open(filename, 'r') as file:
-        return [line.strip('\n') for line in file]
-
-
-def write_smoldyn_simulation_configuration(configuration, filename):
-    ''' Write a configuration for Smoldyn simulation to a file
-
-    Args:
-        configuration
-        filename (:obj:`str`): path to save configuration
-    '''
-    with open(filename, 'w') as file:
-        for line in configuration:
-            file.write(line)
-            file.write('\n')
-
-
-def normalize_smoldyn_simulation_configuration(configuration):
-    ''' Normalize a configuration for a Smoldyn simulation
-
-    Args:
-        configuration (:obj:`list` of :obj:`str`): configuration for a Smoldyn simulation
-    '''
-    # normalize spacing and comments
-    for i_line, line in enumerate(configuration):
-        if '#' in line:
-            cmd, comment = re.split('#+', line, maxsplit=1)
-            cmd = re.sub(' +', ' ', cmd).strip()
-            comment = comment.strip()
-
-            if cmd:
-                if comment:
-                    line = cmd + ' # ' + comment
-                else:
-                    line = cmd
-            else:
-                if comment:
-                    line = '# ' + comment
-                else:
-                    line = ''
-
-        else:
-            line = re.sub(' +', ' ', line).strip()
-
-        configuration[i_line] = line
-
-    # remove end_file and following lines
-    for i_line, line in enumerate(configuration):
-        if re.match(r'^end_file( |$)', line):
-            for i_line_remove in range(len(configuration) - i_line):
-                configuration.pop()
-            break
-
-    # remove empty starting lines
-    for line in list(configuration):
-        if not line:
-            configuration.pop(0)
-        else:
-            break
-
-    # remove empty ending lines
-    for line in reversed(configuration):
-        if not line:
-            configuration.pop()
-        else:
-            break
-
-
-def disable_smoldyn_graphics_in_simulation_configuration(configuration):
-    ''' Turn off graphics in the configuration of a Smoldyn simulation
-
-    Args:
-        configuration (:obj:`list` of :obj:`str`): simulation configuration
-    '''
-    for i_line, line in enumerate(configuration):
-        if line.startswith('graphics '):
-            configuration[i_line] = re.sub(r'^graphics +[a-z_]+', 'graphics none', line)
-
-
-def validate_model_change(sed_model_change):
-    ''' Validate a SED model attribute change to a configuration for a Smoldyn simulation
-
-    ====================================================================  ===================
-    target                                                                newValue
-    ====================================================================  ===================
-    ``define {name}``                                                     float
-    ``difc {species}``                                                    float
-    ``difc {species}({state})``                                           float
-    ``difc_rule {species}({state})``                                      float
-    ``difm {species}``                                                    float[]
-    ``difm {species}({state})``                                           float[]
-    ``difm_rule {species}({state})``                                      float[]
-    ``drift {species}``                                                   float[]
-    ``drift {species}({state})``                                          float[]
-    ``drift_rule {species}({state})``                                     float[]
-    ``surface_drift {species}({state}) {surface} {panel-shape}``          float[]
-    ``surface_drift_rule {species}({state}) {surface} {panel-shape}``     float[]
-    ``killmol {species}({state})``                                        0
-    ``killmolprob {species}({state}) {prob}``                             0
-    ``killmolincmpt {species}({state}) {compartment}``                    0
-    ``killmolinsphere {species}({state}) {surface}``                      0
-    ``killmoloutsidesystem {species}({state})``                           0
-    ``fixmolcount {species}({state})``                                    integer
-    ``fixmolcountincmpt {species}({staet}) {compartment}``                integer
-    ``fixmolcountonsurf {species}({state}) {surface}``                    integer
-    ====================================================================  ===================
-
-    Args:
-        sed_model_change (:obj:`ModelAttributeChange`): SED model change
-
-    Returns:
-        :obj:`SimulationChange`: Smoldyn representation of the model change
-
-    Raises:
-        :obj:`NotImplementedError`: unsupported model change
-    '''
-    # TODO: support additional types of model changes
-
-    target_type, _, target = sed_model_change.target.strip().partition(' ')
-    target_type = target_type.strip()
-    target = re.sub(r' +', ' ', target).strip()
-
-    if target_type in [
-        'killmol', 'killmolprob', 'killmolinsphere', 'killmolincmpt', 'killmoloutsidesystem',
-    ]:
-        # Examples:
-        #   killmol red
-        def new_line_func(new_value):
-            return target_type + ' ' + target
-        execution = SimulationChangeExecution.simulation
-
-    elif target_type in [
-        'fixmolcount', 'fixmolcountonsurf', 'fixmolcountincmpt',
-    ]:
-        # Examples:
-        #   fixmolcount red
-        species_name, species_target_sep, target = target.partition(' ')
-
-        def new_line_func(new_value):
-            return target_type + ' ' + species_name + ' ' + new_value + species_target_sep + target
-
-        execution = SimulationChangeExecution.simulation
-
-    elif target_type in [
-        'define', 'difc', 'difc_rule', 'difm', 'difm_rule',
-        'drift', 'drift_rule', 'surface_drift', 'surface_drift_rule',
-    ]:
-        # Examples:
-        #   define K_FWD 0.001
-        #   difc S 3
-        #   difm red 1 0 0 0 0 0 0 0 2
-        def new_line_func(new_value):
-            return target_type + ' ' + target + ' ' + new_value
-
-        execution = SimulationChangeExecution.preprocessing
-
-    # elif target_type in [
-    #     'mol', 'compartment_mol', 'surface_mol',
-    # ]:
-    #     # Examples:
-    #     #   mol 5 red u
-    #     #   compartment_mol 500 S inside
-    #     #   surface_mol 100 E(front) membrane all all
-    #     def new_line_func(new_value):
-    #         return target_type + ' ' + new_value + ' ' + target
-    #
-    #     execution = SimulationChangeExecution.preprocessing
-
-    # elif target_type in [
-    #     'dim',
-    # ]:
-    #     # Examples:
-    #     #   dim 1
-    #     def new_line_func(new_value):
-    #         return target_type + ' ' + new_value
-    #
-    #     execution = SimulationChangeExecution.preprocessing
-
-    # elif target_type in [
-    #     'boundaries', 'low_wall', 'high_wall',
-    # ]:
-    #     # Examples:
-    #     #   low_wall x -10
-    #     #   high_wall y 10
-    #     def new_line_func(new_value):
-    #         return target_type + ' ' + target + ' ' + new_value
-    #
-    #     execution = SimulationChangeExecution.preprocessing
-
-    else:
-        raise NotImplementedError('Target `{}` is not supported.'.format(sed_model_change.target))
-
-    return SimulationChange(new_line_func, execution)
-
-
-def apply_change_to_smoldyn_simulation(smoldyn_simulation, sed_change, smoldyn_change):
-    ''' Apply a SED model attribute change to a Smoldyn simulation
-
-    Args:
-        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
-        sed_change (:obj:`ModelAttributeChange`): SED model change
-        smoldyn_change (:obj:`SimulationChange`): Smoldyn representation of the model change
-    '''
-    new_value = str(sed_change.new_value).strip()
-    new_line = smoldyn_change.command(new_value)
-    smoldyn_simulation.addCommand(new_line, 'b')
-
-
-def apply_change_to_smoldyn_simulation_configuration(smoldyn_simulation_configuration, sed_change, smoldyn_change):
-    ''' Apply a SED model attribute change to a configuration for a Smoldyn simulation
-
-    Args:
-        smoldyn_simulation_configuration (:obj:`list` of :obj:`str`): configuration for the Smoldyn simulation
-        sed_change (:obj:`ModelAttributeChange`): SED model change
-        smoldyn_change (:obj:`SimulationChange`): Smoldyn representation of the model change
-    '''
-    new_value = str(sed_change.new_value).strip()
-    new_line = smoldyn_change.command(new_value)
-    smoldyn_simulation_configuration.insert(0, new_line)
-
-
-def get_smoldyn_run_timecourse_args(sed_simulation):
-    ''' Get the Smoldyn representation of a SED uniform time course simulation
-
-    Args:
-        sed_simulation (:obj:`UniformTimeCourseSimulation`): SED uniform time course simulation
-
-    Returns:
-        :obj:`dict`: dictionary with keys ``start``, ``stop``, and ``dt`` that captures the Smoldyn
-            representation of the time course
-
-    Raises:
-        :obj:`NotImplementedError`: unsupported timecourse
-    '''
-    number_of_steps = (
-        (
-            sed_simulation.output_end_time - sed_simulation.initial_time
-        ) / (
-            sed_simulation.output_end_time - sed_simulation.output_start_time
-        ) * (
-            sed_simulation.number_of_steps
-        )
-    )
-    if (number_of_steps - int(number_of_steps)) > 1e-8:
-        msg = (
-            'Simulations must specify an integer number of steps, not {}.'
-            '\n  Initial time: {}'
-            '\n  Output start time: {}'
-            '\n  Output end time: {}'
-            '\n  Number of steps (output start to end time): {}'
-        ).format(
-            number_of_steps,
-            sed_simulation.initial_time,
-            sed_simulation.output_start_time,
-            sed_simulation.output_end_time,
-            sed_simulation.number_of_steps,
-        )
-        raise NotImplementedError(msg)
-
-    dt = (sed_simulation.output_end_time - sed_simulation.output_start_time) / sed_simulation.number_of_steps
-
-    return {
-        'start': sed_simulation.initial_time,
-        'stop': sed_simulation.output_end_time,
-        'dt': dt,
-    }
-
-
-def get_smoldyn_instance_attr_or_run_algorithm_parameter_arg(sed_algorithm_parameter_change):
-    ''' Get the Smoldyn representation of a SED uniform time course simulation
-
-    Args:
-        sed_algorithm_parameter_change (:obj:`AlgorithmParameterChange`): SED change to a parameter of an algorithm
-
-    Returns:
-        :obj:`dict`: dictionary with keys ``type``, ``name``, and ``value`` that captures the Smoldyn representation
-            of the algorithm parameter
-
-    Raises:
-        :obj:`ValueError`: unsupported algorithm parameter value
-        :obj:`NotImplementedError`: unsupported algorithm parameter
-    '''
-    parameter_props = KISAO_ALGORITHM_PARAMETERS_MAP.get(sed_algorithm_parameter_change.kisao_id, None)
-    if parameter_props:
-        if not validate_str_value(sed_algorithm_parameter_change.new_value, parameter_props['data_type']):
-            msg = '{} ({}) must be a {}, not `{}`.'.format(
-                parameter_props['name'], sed_algorithm_parameter_change.kisao_id,
-                parameter_props['data_type'].name, sed_algorithm_parameter_change.new_value,
-            )
-            raise ValueError(msg)
-        new_value = parse_value(sed_algorithm_parameter_change.new_value, parameter_props['data_type'])
-
-        return {
-            'type': parameter_props['type'],
-            'name': parameter_props['name'],
-            'value': new_value,
-        }
-
-    else:
-        msg = 'Algorithm parameter `{}` is not supported. The following parameters are supported:{}'.format(
-            sed_algorithm_parameter_change.kisao_id,
-            ''.join('\n  {}: {}'.format(kisao_id, parameter_props['name'])
-                    for kisao_id, parameter_props in KISAO_ALGORITHM_PARAMETERS_MAP.items())
-        )
-        raise NotImplementedError(msg)
-
-
-def add_smoldyn_output_file(configuration_dirname, smoldyn_simulation):
-    ''' Add an output file to a Smoldyn simulation
-
-    Args:
-        configuration_dirname (:obj:`str`): path to the parent directory of the Smoldyn configuration file for the simulation
-        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
-
-    Returns:
-        :obj:`SmoldynOutputFile`: output file
-    '''
-    fid, filename = tempfile.mkstemp(dir=configuration_dirname, suffix='.ssv')
-    os.close(fid)
-    name = os.path.relpath(filename, configuration_dirname)
-    smoldyn_simulation.setOutputFile(name, append=False)
-    smoldyn_simulation.setOutputPath('./')
-    return SmoldynOutputFile(name=name, filename=filename)
-
-
-def add_commands_to_smoldyn_output_file(simulation, output_file, commands):
-    ''' Add commands to a Smoldyn output file
-
-    Args:
-        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
-        smoldyn_output_file (:obj:`SmoldynOutputFile`): Smoldyn output file
-        commands (:obj:`list` of :obj`SmoldynCommand`): Smoldyn commands
-    '''
-    for command in commands:
-        simulation.addCommand(command.command + ' ' + output_file.name, command.type)
-
-
-def validate_variables(variables):
-    ''' Validate SED variables
-
-    =============================================================================================================================================  ===========================================================================================================================================  ===========================================
-    Smoldyn output file                                                                                                                            SED variable target                                                                                                                          Shape
-    =============================================================================================================================================  ===========================================================================================================================================  ===========================================
-    ``molcount``                                                                                                                                   ``molcount {species}``                                                                                                                       (numberOfSteps + 1,)
-    ``molcountspecies {species}({state})``                                                                                                         ``molcountspecies {species}({state})``                                                                                                       (numberOfSteps + 1,)
-    ``molcountspecieslist {species}({state})+``                                                                                                    ``molcountspecies {species}({state})``                                                                                                       (numberOfSteps + 1,)
-    ``molcountinbox {low-x} {hi-x}``                                                                                                               ``molcountinbox {species} {low-x} {hi-x}``                                                                                                   (numberOfSteps + 1,)
-    ``molcountinbox {low-x} {hi-x} {low-y} {hi-y}``                                                                                                ``molcountinbox {species} {low-x} {hi-x} {low-y} {hi-y}``                                                                                    (numberOfSteps + 1,)
-    ``molcountinbox {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z}``                                                                                 ``molcountinbox {species} {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z}``                                                                     (numberOfSteps + 1,)
-    ``molcountincmpt {compartment}``                                                                                                               ``molcountincmpt {species} {compartment}``                                                                                                   (numberOfSteps + 1,)
-    ``molcountincmpts {compartment}+``                                                                                                             ``molcountincmpt {species} {compartment}``                                                                                                   (numberOfSteps + 1,)
-    ``molcountincmpt2 {compartment} {state}``                                                                                                      ``molcountincmpt2 {species} {compartment} {state}``                                                                                          (numberOfSteps + 1,)
-    ``molcountonsurf {surface}``                                                                                                                   ``molcountonsurf {species} {surface}``                                                                                                       (numberOfSteps + 1,)
-    ``molcountspace {species}({state}) {axis} {low} {hi} {bins} 0``                                                                                ``molcountspace {species}({state}) {axis} {low} {hi} {bins}``                                                                                (numberOfSteps + 1, bins)
-    ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi} 0``                                                                     ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi}``                                                                     (numberOfSteps + 1, bins)
-    ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi} {low} {hi} 0``                                                          ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi} {low} {hi}``                                                          (numberOfSteps + 1, bins)
-    ``molcountspace2d {species}({state}) z {low-x} {hi-x} {bins-x} {low-y} {hi-y} {bins-y} 0``                                                     ``molcountspace2d {species}({state}) z {low-x} {hi-x} {bins-x} {low-y} {hi-y} {bins-y}``                                                     (numberOfSteps + 1, bins-x, bins-y)
-    ``molcountspace2d {species}({state}) {axis} {low-1} {hi-1} {bins-1} {low-2} {hi-2} {bins-2} {low-3} {hi-3} 0``                                 ``molcountspace2d {species}({state}) {axis} {low-1} {hi-1} {bins-1} {low-2} {hi-2} {bins-3} {low-3} {hi-3}``                                 (numberOfSteps + 1, bins-1, bins-2)
-    ``molcountspaceradial {species}({state}) {center-x} {radius} {bins} 0``                                                                        ``molcountspaceradial {species}({state}) {center-x} {radius} {bins}``                                                                        (numberOfSteps + 1, bins)
-    ``molcountspaceradial {species}({state}) {center-x} {center-y} {radius} {bins} 0``                                                             ``molcountspaceradial {species}({state}) {center-x} {center-y} {radius} {bins}``                                                             (numberOfSteps + 1, bins)
-    ``molcountspaceradial {species}({state}) {center-x} {center-y} {center-z} {radius} {bins} 0``                                                  ``molcountspaceradial {species}({state}) {center-x} {center-y} {center-z} {radius} {bins}``                                                  (numberOfSteps + 1, bins)
-    ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {pole-x} {pole-y} {radius-min} {radius-max} {bins} 0``                      ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {pole-x} {pole-y} {radius-min} {radius-max} {bins}``                      (numberOfSteps + 1, bins)
-    ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {center-z} {pole-x} {pole-y} {pole-z} {radius-min} {radius-max} {bins} 0``  ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {center-z} {pole-x} {pole-y} {pole-z} {radius-min} {radius-max} {bins}``  (numberOfSteps + 1, bins)
-    ``radialdistribution {species-1}({state-1}) {species-2}({state-2}) {radius} {bins} 0``                                                         ``radialdistribution {species-1}({state-1}) {species-2}({state-2}) {radius} {bins}``                                                         (numberOfSteps + 1, bins)
-    ``radialdistribution2 {species-1}({state-1}) {species-2}({state-2}) {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z} {radius} {bins} 0``           ``radialdistribution2 {species-1}({state-1}) {species-2}({state-2}) {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z} {radius} {bins}``           (numberOfSteps + 1, bins)
-    =============================================================================================================================================   ==========================================================================================================================================  ===========================================
-
-    Args:
-        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
-
-    Returns:
-        :obj:`dict`: dictionary that maps variable targets and symbols to Smoldyn output commands
-    '''
-    # TODO: support additional kinds of outputs
-
-    variable_output_cmd_map = {}
-
-    invalid_symbols = []
-    invalid_targets = []
-
-    for variable in variables:
-        if variable.symbol:
-            if variable.symbol == Symbol.time.value:
-                output_command_args = 'molcount'
-                include_header = True
-                shape = None
-                results_slicer = functools.partial(results_key_slicer, key='time')
-
-            else:
-                invalid_symbols.append('{}: {}'.format(variable.id, variable.symbol))
-                output_command_args = None
-                include_header = None
-
-        else:
-            output_command, _, output_args = re.sub(r' +', ' ', variable.target).partition(' ')
-
-            if output_command in ['molcount', 'molcountinbox', 'molcountincmpt', 'molcountincmpt2', 'molcountonsurf']:
-                species_name, _, output_args = output_args.partition(' ')
-                output_command_args = output_command + ' ' + output_args
-                include_header = True
-                shape = None
-                results_slicer = functools.partial(results_key_slicer, key=species_name)
-
-            elif output_command in ['molcountspecies']:
-                output_command_args = output_command + ' ' + output_args
-                include_header = False
-                shape = None
-                results_slicer = results_array_slicer
-
-            elif output_command in ['molcountspace', 'molcountspaceradial',
-                                    'molcountspacepolarangle', 'radialdistribution', 'radialdistribution2']:
-                output_command_args = output_command + ' ' + output_args + ' 0'
-                include_header = False
-                shape = None
-                results_slicer = results_matrix_slicer
-
-            elif output_command in ['molcountspace2d']:
-                output_command_args = output_command + ' ' + output_args + ' 0'
-                include_header = False
-                output_args_list = output_args.split(' ')
-                if len(output_args_list) == 8:
-                    shape = (int(output_args_list[-4]), int(output_args_list[-1]))
-                else:
-                    shape = (int(output_args_list[-6]), int(output_args_list[-3]))
-                results_slicer = None
-
-            else:
-                invalid_targets.append('{}: {}'.format(variable.id, variable.target))
-                output_command_args = None
-
-        if output_command_args is not None:
-            output_command_args = output_command_args.strip()
-            variable_output_cmd_map[(variable.target, variable.symbol)] = (output_command_args, include_header, shape, results_slicer)
-
-    if invalid_symbols:
-        msg = '{} symbols cannot be recorded:\n  {}\n\nThe following symbols can be recorded:\n  {}'.format(
-            len(invalid_symbols),
-            '\n  '.join(sorted(invalid_symbols)),
-            '\n  '.join(sorted([Symbol.time.value])),
-        )
-        raise ValueError(msg)
-
-    if invalid_targets:
-        valid_target_output_commands = [
-            'molcount',
-
-            'molcount', 'molcountinbox', 'molcountincmpt', 'molcountincmpt2', 'molcountonsurf',
-
-            'molcountspace', 'molcountspaceradial',
-            'molcountspacepolarangle', 'radialdistribution', 'radialdistribution2',
-
-            'molcountspace2d',
-        ]
-
-        msg = '{} targets cannot be recorded:\n  {}\n\nTargets are supported for the following output commands:\n  {}'.format(
-            len(invalid_targets),
-            '\n  '.join(sorted(invalid_targets)),
-            '\n  '.join(sorted(set(valid_target_output_commands))),
-        )
-        raise NotImplementedError(msg)
-
-    return variable_output_cmd_map
-
-
-def results_key_slicer(results, key):
-    """ Get the results for a key from a set of results
-
-    Args:
-        results (:obj:`pandas.DataFrame`): set of results
-
-    Returns:
-        :obj:`pandas.DataFrame`: results for a key
-    """
-    return results.get(key, None)
-
-
-def results_array_slicer(results):
-    """ Extract an array of results from a matrix of time and results
-
-    Args:
-        results (:obj:`pandas.DataFrame`): matrix of time and results
-
-    Returns:
-        :obj:`pandas.DataFrame`: results
-    """
-    return results.iloc[:, 1]
-
-
-def results_matrix_slicer(results):
-    """ Extract a matrix array of results from a matrix of time and results
-
-    Args:
-        results (:obj:`pandas.DataFrame`): matrix of time and results
-
-    Returns:
-        :obj:`pandas.DataFrame`: results
-    """
-    return results.iloc[:, 1:]
-
-
-def add_smoldyn_output_files_for_sed_variables(configuration_dirname, variables, variable_output_cmd_map, smoldyn_simulation):
-    ''' Add Smoldyn output files for capturing each SED variable
-
-    Args:
-        configuration_dirname (:obj:`str`): path to the parent directory of the Smoldyn configuration file for the simulation
-        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
-        variable_output_cmd_map (:obj:`dict`): dictionary that maps variable targets and symbols to Smoldyn output commands
-        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
-
-    Returns:
-        :obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`: Smoldyn output files
-    '''
-    smoldyn_output_files = {}
-
-    output_cmds = set()
-    for variable in variables:
-        output_cmds.add(variable_output_cmd_map[(variable.target, variable.symbol)])
-
-    for command, include_header, _, _ in output_cmds:
-        add_smoldyn_output_file_for_output(configuration_dirname, smoldyn_simulation,
-                                           command, include_header,
-                                           smoldyn_output_files)
-    # return output files
-    return smoldyn_output_files
-
-
-def add_smoldyn_output_file_for_output(configuration_dirname, smoldyn_simulation,
-                                       smoldyn_output_command, include_header, smoldyn_output_files):
-    ''' Add a Smoldyn output file for molecule counts
-
-    Args:
-        configuration_dirname (:obj:`str`): path to the parent directory of the Smoldyn configuration file for the simulation
-        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
-        smoldyn_output_command (:obj:`str`): Smoldyn output command (e.g., ``molcount``)
-        include_header (:obj:`bool`): whether to include a header
-        smoldyn_output_files (:obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`): Smoldyn output files
-    '''
-    smoldyn_output_files[smoldyn_output_command] = add_smoldyn_output_file(configuration_dirname, smoldyn_simulation)
-
-    commands = []
-    if include_header:
-        commands.append(SmoldynCommand('molcountheader', 'B'))
-    commands.append(SmoldynCommand(smoldyn_output_command, 'E'))
-
-    add_commands_to_smoldyn_output_file(
-        smoldyn_simulation,
-        smoldyn_output_files[smoldyn_output_command],
-        commands,
-    )
-
-
-def get_variable_results(number_of_steps, variables, variable_output_cmd_map, smoldyn_output_files):
-    ''' Get the result of each SED variable
-
-    Args:
-        number_of_steps (:obj:`int`): number of steps
-        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
-        variable_output_cmd_map (:obj:`dict`): dictionary that maps variable targets and symbols to Smoldyn output commands
-        smoldyn_output_files (:obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`): Smoldyn output files
-
-    Returns:
-        :obj:`VariableResults`: result of each SED variable
-
-    Raises:
-        :obj:`ValueError`: unsupported results
-    '''
-    smoldyn_results = {}
-
-    missing_variables = []
-
-    variable_results = VariableResults()
-    for variable in variables:
-        output_command_args, _, shape, results_slicer = variable_output_cmd_map[(variable.target, variable.symbol)]
-        variable_result = get_smoldyn_output(output_command_args, True, shape, smoldyn_output_files, smoldyn_results)
-        if results_slicer:
-            variable_result = results_slicer(variable_result)
-
-        if variable_result is None:
-            missing_variables.append('{}: {}: {}'.format(variable.id, 'target', variable.target))
-        else:
-            if variable_result.ndim == 1:
-                variable_results[variable.id] = variable_result.to_numpy()[-(number_of_steps + 1):, ]
-            elif variable_result.ndim == 2:
-                variable_results[variable.id] = variable_result.to_numpy()[-(number_of_steps + 1):, :]
-            else:
-                variable_results[variable.id] = variable_result[-(number_of_steps + 1):, :, :]
-
-    if missing_variables:
-        msg = '{} variables could not be recorded:\n  {}'.format(
-            len(missing_variables),
-            '\n  '.join(missing_variables),
-        )
-        raise ValueError(msg)
-
-    return variable_results
-
-
-def get_smoldyn_output(smoldyn_output_command, has_header, three_d_shape, smoldyn_output_files, smoldyn_results):
-    ''' Get the simulated count of each molecule
-
-    Args:
-        smoldyn_output_command (:obj:`str`): Smoldyn output command (e.g., ``molcount``)
-        has_header (:obj:`bool`): whether to include a header
-        three_d_shape (:obj:`tuple` of :obj:`int`): dimensions of the output
-        smoldyn_output_files (:obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`): Smoldyn output files
-        smoldyn_results (:obj:`dict`)
-
-    Returns:
-        :obj:`pandas.DataFrame` or :obj:`numpy.ndarray`: results
-    '''
-    smoldyn_output_command = smoldyn_output_command.strip()
-    if smoldyn_output_command not in smoldyn_results:
-        smoldyn_output_file = smoldyn_output_files[smoldyn_output_command]
-        if three_d_shape:
-            with open(smoldyn_output_file.filename, 'r') as file:
-                data_list = []
-
-                i_line = 0
-                for line in file:
-                    if i_line % (three_d_shape[1] + 1) == 0:
-                        time_point_data = []
-                    else:
-                        profile = [int(el) for el in line.split(' ')]
-                        time_point_data.append(profile)
-
-                        if i_line % (three_d_shape[1] + 1) == three_d_shape[1]:
-                            data_list.append(time_point_data)
-
-                    i_line += 1
-
-            smoldyn_results[smoldyn_output_command] = numpy.array(data_list).transpose((0, 2, 1))
-
-        else:
-            smoldyn_results[smoldyn_output_command] = pandas.read_csv(smoldyn_output_file.filename, sep=' ')
-
-    return smoldyn_results[smoldyn_output_command]
+''' Methods for executing COMBINE archives and SED-ML files involving simulations of models encoded in Smoldyn
+
+    Information about encoding Smoldyn simulations into SED-ML files and COMBINE archives is available at
+    `https://github.com/ssandrews/Smoldyn/blob/master/Using-Smoldyn-with-SED-ML-COMBINE-BioSimulators.md <https://github.com/ssandrews/Smoldyn/blob/master/Using-Smoldyn-with-SED-ML-COMBINE-BioSimulators.md>`_.
+'''
+
+__author__ = 'Jonathan Karr'
+__email__ = 'karr@mssm.edu'
+
+__all__ = [
+    'exec_sedml_docs_in_combine_archive',
+    'exec_sed_task',
+]
+
+from .data_model import (SmoldynCommand, SmoldynOutputFile, SimulationChange, SimulationChangeExecution, AlgorithmParameterType,
+                         KISAO_ALGORITHMS_MAP, KISAO_ALGORITHM_PARAMETERS_MAP)
+from biosimulators_utils.combine.exec import exec_sedml_docs_in_archive
+from biosimulators_utils.config import get_config, Config  # noqa: F401
+from biosimulators_utils.log.data_model import CombineArchiveLog, TaskLog, StandardOutputErrorCapturerLevel  # noqa: F401
+from biosimulators_utils.viz.data_model import VizFormat  # noqa: F401
+from biosimulators_utils.report.data_model import ReportFormat, VariableResults, SedDocumentResults  # noqa: F401
+from biosimulators_utils.sedml import validation
+from biosimulators_utils.sedml.data_model import (Task, ModelLanguage, ModelAttributeChange,  # noqa: F401
+                                                  UniformTimeCourseSimulation, AlgorithmParameterChange, Variable,
+                                                  Symbol)
+from biosimulators_utils.sedml.exec import exec_sed_doc as base_exec_sed_doc
+from biosimulators_utils.utils.core import validate_str_value, parse_value, raise_errors_warnings
+from smoldyn import smoldyn
+import functools
+import os
+import numpy
+import pandas
+import re
+import tempfile
+import types  # noqa: F401
+
+__all__ = ['exec_sedml_docs_in_combine_archive', 'exec_sed_task', 'exec_sed_doc', 'preprocess_sed_task']
+
+
+def exec_sedml_docs_in_combine_archive(archive_filename, out_dir, config=None):
+    ''' Execute the SED tasks defined in a COMBINE/OMEX archive and save the outputs
+
+    Args:
+        archive_filename (:obj:`str`): path to COMBINE/OMEX archive
+        out_dir (:obj:`str`): path to store the outputs of the archive
+
+            * CSV: directory in which to save outputs to files
+              ``{ out_dir }/{ relative-path-to-SED-ML-file-within-archive }/{ report.id }.csv``
+            * HDF5: directory in which to save a single HDF5 file (``{ out_dir }/reports.h5``),
+              with reports at keys ``{ relative-path-to-SED-ML-file-within-archive }/{ report.id }`` within the HDF5 file
+
+        config (:obj:`Config`, optional): BioSimulators common configuration
+
+    Returns:
+        :obj:`tuple`:
+
+            * :obj:`SedDocumentResults`: results
+            * :obj:`CombineArchiveLog`: log
+    '''
+    return exec_sedml_docs_in_archive(exec_sed_doc, archive_filename, out_dir,
+                                      apply_xml_model_changes=False,
+                                      config=config)
+
+
+def exec_sed_doc(doc, working_dir, base_out_path, rel_out_path=None,
+                 apply_xml_model_changes=True,
+                 log=None, indent=0, pretty_print_modified_xml_models=False,
+                 log_level=StandardOutputErrorCapturerLevel.c, config=None):
+    """ Execute the tasks specified in a SED document and generate the specified outputs
+
+    Args:
+        doc (:obj:`SedDocument` or :obj:`str`): SED document or a path to SED-ML file which defines a SED document
+        working_dir (:obj:`str`): working directory of the SED document (path relative to which models are located)
+
+        base_out_path (:obj:`str`): path to store the outputs
+
+            * CSV: directory in which to save outputs to files
+              ``{base_out_path}/{rel_out_path}/{report.id}.csv``
+            * HDF5: directory in which to save a single HDF5 file (``{base_out_path}/reports.h5``),
+              with reports at keys ``{rel_out_path}/{report.id}`` within the HDF5 file
+
+        rel_out_path (:obj:`str`, optional): path relative to :obj:`base_out_path` to store the outputs
+        apply_xml_model_changes (:obj:`bool`, optional): if :obj:`True`, apply any model changes specified in the SED-ML file before
+            calling :obj:`task_executer`.
+        log (:obj:`SedDocumentLog`, optional): log of the document
+        indent (:obj:`int`, optional): degree to indent status messages
+        pretty_print_modified_xml_models (:obj:`bool`, optional): if :obj:`True`, pretty print modified XML models
+        log_level (:obj:`StandardOutputErrorCapturerLevel`, optional): level at which to log output
+        config (:obj:`Config`, optional): BioSimulators common configuration
+        simulator_config (:obj:`SimulatorConfig`, optional): tellurium configuration
+
+    Returns:
+        :obj:`tuple`:
+
+            * :obj:`ReportResults`: results of each report
+            * :obj:`SedDocumentLog`: log of the document
+    """
+    return base_exec_sed_doc(exec_sed_task, doc, working_dir, base_out_path,
+                             rel_out_path=rel_out_path,
+                             apply_xml_model_changes=apply_xml_model_changes,
+                             log=log,
+                             indent=indent,
+                             pretty_print_modified_xml_models=pretty_print_modified_xml_models,
+                             log_level=log_level,
+                             config=config)
+
+
+def exec_sed_task(task, variables, preprocessed_task=None, log=None, config=None):
+    ''' Execute a task and save its results
+
+    Args:
+       task (:obj:`Task`): task
+       variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
+       preprocessed_task (:obj:`dict`, optional): preprocessed information about the task, including possible
+            model changes and variables. This can be used to avoid repeatedly executing the same initialization
+            for repeated calls to this method.
+       log (:obj:`TaskLog`, optional): log for the task
+       config (:obj:`Config`, optional): BioSimulators common configuration
+
+    Returns:
+        :obj:`tuple`:
+
+            :obj:`VariableResults`: results of variables
+            :obj:`TaskLog`: log
+    '''
+    if not config:
+        config = get_config()
+
+    if config.LOG and not log:
+        log = TaskLog()
+
+    sed_model_changes = task.model.changes
+    sed_simulation = task.simulation
+
+    if preprocessed_task is None:
+        preprocessed_task = preprocess_sed_task(task, variables, config=config)
+        sed_model_changes = list(filter(lambda change: change.target in preprocessed_task['sed_smoldyn_simulation_change_map'],
+                                        sed_model_changes))
+
+    # read Smoldyn configuration
+    smoldyn_simulation = preprocessed_task['simulation']
+
+    # apply model changes to the Smoldyn configuration
+    sed_smoldyn_simulation_change_map = preprocessed_task['sed_smoldyn_simulation_change_map']
+    for change in sed_model_changes:
+        smoldyn_change = sed_smoldyn_simulation_change_map.get(change.target, None)
+        if smoldyn_change is None or smoldyn_change.execution != SimulationChangeExecution.simulation:
+            raise NotImplementedError('Target `{}` can only be changed during simulation preprocessing.'.format(change.target))
+        apply_change_to_smoldyn_simulation(
+            smoldyn_simulation, change, smoldyn_change)
+
+    # get the Smoldyn representation of the SED uniform time course simulation
+    smoldyn_simulation_run_timecourse_args = get_smoldyn_run_timecourse_args(sed_simulation)
+
+    # execute the simulation
+    smoldyn_run_args = dict(
+        **smoldyn_simulation_run_timecourse_args,
+        **preprocessed_task['simulation_run_alg_param_args'],
+    )
+    smoldyn_simulation.run(**smoldyn_run_args, overwrite=True, display=False, quit_at_end=False)
+
+    # get the result of each SED variable
+    variable_output_cmd_map = preprocessed_task['variable_output_cmd_map']
+    smoldyn_output_files = preprocessed_task['output_files']
+    variable_results = get_variable_results(sed_simulation.number_of_steps, variables, variable_output_cmd_map, smoldyn_output_files)
+
+    # cleanup output files
+    for smoldyn_output_file in smoldyn_output_files.values():
+        os.remove(smoldyn_output_file.filename)
+
+    # log simulation
+    if config.LOG:
+        log.algorithm = sed_simulation.algorithm.kisao_id
+        log.simulator_details = {
+            'class': 'smoldyn.Simulation',
+            'instanceAttributes': preprocessed_task['simulation_attrs'],
+            'method': 'run',
+            'methodArguments': smoldyn_run_args,
+        }
+
+    # return the values of the variables and log
+    return variable_results, log
+
+
+def preprocess_sed_task(task, variables, config=None):
+    """ Preprocess a SED task, including its possible model changes and variables. This is useful for avoiding
+    repeatedly initializing tasks on repeated calls of :obj:`exec_sed_task`.
+
+    Args:
+        task (:obj:`Task`): task
+        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
+        config (:obj:`Config`, optional): BioSimulators common configuration
+
+    Returns:
+        :obj:`dict`: preprocessed information about the task
+    """
+    config = config or get_config()
+
+    sed_model = task.model
+    sed_simulation = task.simulation
+
+    if config.VALIDATE_SEDML:
+        raise_errors_warnings(validation.validate_task(task),
+                              error_summary='Task `{}` is invalid.'.format(task.id))
+        raise_errors_warnings(validation.validate_model_language(sed_model.language, ModelLanguage.Smoldyn),
+                              error_summary='Language for model `{}` is not supported.'.format(sed_model.id))
+        raise_errors_warnings(validation.validate_model_change_types(sed_model.changes, (ModelAttributeChange, )),
+                              error_summary='Changes for model `{}` are not supported.'.format(sed_model.id))
+        raise_errors_warnings(*validation.validate_model_changes(sed_model),
+                              error_summary='Changes for model `{}` are invalid.'.format(sed_model.id))
+        raise_errors_warnings(validation.validate_simulation_type(sed_simulation, (UniformTimeCourseSimulation, )),
+                              error_summary='{} `{}` is not supported.'.format(sed_simulation.__class__.__name__, sed_simulation.id))
+        raise_errors_warnings(*validation.validate_simulation(sed_simulation),
+                              error_summary='Simulation `{}` is invalid.'.format(sed_simulation.id))
+        raise_errors_warnings(*validation.validate_data_generator_variables(variables),
+                              error_summary='Data generator variables for task `{}` are invalid.'.format(task.id))
+
+    if sed_simulation.algorithm.kisao_id not in KISAO_ALGORITHMS_MAP:
+        msg = 'Algorithm `{}` is not supported. The following algorithms are supported:{}'.format(
+            sed_simulation.algorithm.kisao_id,
+            ''.join('\n  {}: {}'.format(kisao_id, alg_props['name']) for kisao_id, alg_props in KISAO_ALGORITHMS_MAP.items())
+        )
+        raise NotImplementedError(msg)
+
+    # read Smoldyn configuration
+    simulation_configuration = read_smoldyn_simulation_configuration(sed_model.source)
+    normalize_smoldyn_simulation_configuration(simulation_configuration)
+
+    # turn off Smoldyn's graphics
+    disable_smoldyn_graphics_in_simulation_configuration(simulation_configuration)
+
+    # preprocess model changes
+    sed_smoldyn_preprocessing_change_map = {}
+    sed_smoldyn_simulation_change_map = {}
+    for change in sed_model.changes:
+        smoldyn_change = validate_model_change(change)
+
+        if smoldyn_change.execution == SimulationChangeExecution.preprocessing:
+            sed_smoldyn_preprocessing_change_map[change] = smoldyn_change
+        else:
+            sed_smoldyn_simulation_change_map[change.target] = smoldyn_change
+
+    # apply preprocessing-time changes
+    for change, smoldyn_change in sed_smoldyn_preprocessing_change_map.items():
+        apply_change_to_smoldyn_simulation_configuration(
+            simulation_configuration, change, smoldyn_change)
+
+    # write the modified Smoldyn configuration to a temporary file
+    fid, smoldyn_configuration_filename = tempfile.mkstemp(suffix='.txt')
+    os.close(fid)
+    write_smoldyn_simulation_configuration(simulation_configuration, smoldyn_configuration_filename)
+
+    # initialize a simulation from the Smoldyn file
+    smoldyn_simulation = init_smoldyn_simulation_from_configuration_file(smoldyn_configuration_filename)
+
+    # clean up temporary file
+    os.remove(smoldyn_configuration_filename)
+
+    # apply the SED algorithm parameters to the Smoldyn simulation and to the arguments to its ``run`` method
+    smoldyn_simulation_attrs = {}
+    smoldyn_simulation_run_alg_param_args = {}
+    for sed_algorithm_parameter_change in sed_simulation.algorithm.changes:
+        val = get_smoldyn_instance_attr_or_run_algorithm_parameter_arg(sed_algorithm_parameter_change)
+        if val['type'] == AlgorithmParameterType.run_argument:
+            smoldyn_simulation_run_alg_param_args[val['name']] = val['value']
+        else:
+            smoldyn_simulation_attrs[val['name']] = val['value']
+
+    # apply the SED algorithm parameters to the Smoldyn simulation and to the arguments to its ``run`` method
+    for attr_name, value in smoldyn_simulation_attrs.items():
+        setter = getattr(smoldyn_simulation, attr_name)
+        setter(value)
+
+    # validate SED variables
+    variable_output_cmd_map = validate_variables(variables)
+
+    # Setup Smoldyn output files for the SED variables
+    smoldyn_configuration_dirname = os.path.dirname(smoldyn_configuration_filename)
+    smoldyn_output_files = add_smoldyn_output_files_for_sed_variables(
+        smoldyn_configuration_dirname, variables, variable_output_cmd_map, smoldyn_simulation)
+
+    # return preprocessed information
+    return {
+        'simulation': smoldyn_simulation,
+        'simulation_attrs': smoldyn_simulation_attrs,
+        'simulation_run_alg_param_args': smoldyn_simulation_run_alg_param_args,
+        'sed_smoldyn_simulation_change_map': sed_smoldyn_simulation_change_map,
+        'variable_output_cmd_map': variable_output_cmd_map,
+        'output_files': smoldyn_output_files,
+    }
+
+
+def init_smoldyn_simulation_from_configuration_file(filename):
+    ''' Initialize a simulation for a Smoldyn model from a file
+
+    Args:
+        filename (:obj:`str`): path to model file
+
+    Returns:
+        :obj:`smoldyn.Simulation`: simulation
+    '''
+    if not os.path.isfile(filename):
+        raise FileNotFoundError('Model source `{}` is not a file.'.format(filename))
+
+    smoldyn_simulation = smoldyn.Simulation.fromFile(filename)
+    if not smoldyn_simulation.getSimPtr():
+        error_code, error_msg = smoldyn.getError()
+        msg = 'Model source `{}` is not a valid Smoldyn file.\n\n  {}: {}'.format(
+            filename, error_code.name[0].upper() + error_code.name[1:], error_msg.replace('\n', '\n  '))
+        raise ValueError(msg)
+
+    return smoldyn_simulation
+
+
+def read_smoldyn_simulation_configuration(filename):
+    ''' Read a configuration for a Smoldyn simulation
+
+    Args:
+        filename (:obj:`str`): path to model file
+
+    Returns:
+        :obj:`list` of :obj:`str`: simulation configuration
+    '''
+    with open(filename, 'r') as file:
+        return [line.strip('\n') for line in file]
+
+
+def write_smoldyn_simulation_configuration(configuration, filename):
+    ''' Write a configuration for Smoldyn simulation to a file
+
+    Args:
+        configuration
+        filename (:obj:`str`): path to save configuration
+    '''
+    with open(filename, 'w') as file:
+        for line in configuration:
+            file.write(line)
+            file.write('\n')
+
+
+def normalize_smoldyn_simulation_configuration(configuration):
+    ''' Normalize a configuration for a Smoldyn simulation
+
+    Args:
+        configuration (:obj:`list` of :obj:`str`): configuration for a Smoldyn simulation
+    '''
+    # normalize spacing and comments
+    for i_line, line in enumerate(configuration):
+        if '#' in line:
+            cmd, comment = re.split('#+', line, maxsplit=1)
+            cmd = re.sub(' +', ' ', cmd).strip()
+            comment = comment.strip()
+
+            if cmd:
+                if comment:
+                    line = cmd + ' # ' + comment
+                else:
+                    line = cmd
+            else:
+                if comment:
+                    line = '# ' + comment
+                else:
+                    line = ''
+
+        else:
+            line = re.sub(' +', ' ', line).strip()
+
+        configuration[i_line] = line
+
+    # remove end_file and following lines
+    for i_line, line in enumerate(configuration):
+        if re.match(r'^end_file( |$)', line):
+            for i_line_remove in range(len(configuration) - i_line):
+                configuration.pop()
+            break
+
+    # remove empty starting lines
+    for line in list(configuration):
+        if not line:
+            configuration.pop(0)
+        else:
+            break
+
+    # remove empty ending lines
+    for line in reversed(configuration):
+        if not line:
+            configuration.pop()
+        else:
+            break
+
+
+def disable_smoldyn_graphics_in_simulation_configuration(configuration):
+    ''' Turn off graphics in the configuration of a Smoldyn simulation
+
+    Args:
+        configuration (:obj:`list` of :obj:`str`): simulation configuration
+    '''
+    for i_line, line in enumerate(configuration):
+        if line.startswith('graphics '):
+            configuration[i_line] = re.sub(r'^graphics +[a-z_]+', 'graphics none', line)
+
+
+def validate_model_change(sed_model_change):
+    ''' Validate a SED model attribute change to a configuration for a Smoldyn simulation
+
+    ====================================================================  ===================
+    target                                                                newValue
+    ====================================================================  ===================
+    ``define {name}``                                                     float
+    ``difc {species}``                                                    float
+    ``difc {species}({state})``                                           float
+    ``difc_rule {species}({state})``                                      float
+    ``difm {species}``                                                    float[]
+    ``difm {species}({state})``                                           float[]
+    ``difm_rule {species}({state})``                                      float[]
+    ``drift {species}``                                                   float[]
+    ``drift {species}({state})``                                          float[]
+    ``drift_rule {species}({state})``                                     float[]
+    ``surface_drift {species}({state}) {surface} {panel-shape}``          float[]
+    ``surface_drift_rule {species}({state}) {surface} {panel-shape}``     float[]
+    ``killmol {species}({state})``                                        0
+    ``killmolprob {species}({state}) {prob}``                             0
+    ``killmolincmpt {species}({state}) {compartment}``                    0
+    ``killmolinsphere {species}({state}) {surface}``                      0
+    ``killmoloutsidesystem {species}({state})``                           0
+    ``fixmolcount {species}({state})``                                    integer
+    ``fixmolcountincmpt {species}({staet}) {compartment}``                integer
+    ``fixmolcountonsurf {species}({state}) {surface}``                    integer
+    ====================================================================  ===================
+
+    Args:
+        sed_model_change (:obj:`ModelAttributeChange`): SED model change
+
+    Returns:
+        :obj:`SimulationChange`: Smoldyn representation of the model change
+
+    Raises:
+        :obj:`NotImplementedError`: unsupported model change
+    '''
+    # TODO: support additional types of model changes
+
+    target_type, _, target = sed_model_change.target.strip().partition(' ')
+    target_type = target_type.strip()
+    target = re.sub(r' +', ' ', target).strip()
+
+    if target_type in [
+        'killmol', 'killmolprob', 'killmolinsphere', 'killmolincmpt', 'killmoloutsidesystem',
+    ]:
+        # Examples:
+        #   killmol red
+        def new_line_func(new_value):
+            return target_type + ' ' + target
+        execution = SimulationChangeExecution.simulation
+
+    elif target_type in [
+        'fixmolcount', 'fixmolcountonsurf', 'fixmolcountincmpt',
+    ]:
+        # Examples:
+        #   fixmolcount red
+        species_name, species_target_sep, target = target.partition(' ')
+
+        def new_line_func(new_value):
+            return target_type + ' ' + species_name + ' ' + new_value + species_target_sep + target
+
+        execution = SimulationChangeExecution.simulation
+
+    elif target_type in [
+        'define', 'difc', 'difc_rule', 'difm', 'difm_rule',
+        'drift', 'drift_rule', 'surface_drift', 'surface_drift_rule',
+    ]:
+        # Examples:
+        #   define K_FWD 0.001
+        #   difc S 3
+        #   difm red 1 0 0 0 0 0 0 0 2
+        def new_line_func(new_value):
+            return target_type + ' ' + target + ' ' + new_value
+
+        execution = SimulationChangeExecution.preprocessing
+
+    # elif target_type in [
+    #     'mol', 'compartment_mol', 'surface_mol',
+    # ]:
+    #     # Examples:
+    #     #   mol 5 red u
+    #     #   compartment_mol 500 S inside
+    #     #   surface_mol 100 E(front) membrane all all
+    #     def new_line_func(new_value):
+    #         return target_type + ' ' + new_value + ' ' + target
+    #
+    #     execution = SimulationChangeExecution.preprocessing
+
+    # elif target_type in [
+    #     'dim',
+    # ]:
+    #     # Examples:
+    #     #   dim 1
+    #     def new_line_func(new_value):
+    #         return target_type + ' ' + new_value
+    #
+    #     execution = SimulationChangeExecution.preprocessing
+
+    # elif target_type in [
+    #     'boundaries', 'low_wall', 'high_wall',
+    # ]:
+    #     # Examples:
+    #     #   low_wall x -10
+    #     #   high_wall y 10
+    #     def new_line_func(new_value):
+    #         return target_type + ' ' + target + ' ' + new_value
+    #
+    #     execution = SimulationChangeExecution.preprocessing
+
+    else:
+        raise NotImplementedError('Target `{}` is not supported.'.format(sed_model_change.target))
+
+    return SimulationChange(new_line_func, execution)
+
+
+def apply_change_to_smoldyn_simulation(smoldyn_simulation, sed_change, smoldyn_change):
+    ''' Apply a SED model attribute change to a Smoldyn simulation
+
+    Args:
+        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
+        sed_change (:obj:`ModelAttributeChange`): SED model change
+        smoldyn_change (:obj:`SimulationChange`): Smoldyn representation of the model change
+    '''
+    new_value = str(sed_change.new_value).strip()
+    new_line = smoldyn_change.command(new_value)
+    smoldyn_simulation.addCommand(new_line, 'b')
+
+
+def apply_change_to_smoldyn_simulation_configuration(smoldyn_simulation_configuration, sed_change, smoldyn_change):
+    ''' Apply a SED model attribute change to a configuration for a Smoldyn simulation
+
+    Args:
+        smoldyn_simulation_configuration (:obj:`list` of :obj:`str`): configuration for the Smoldyn simulation
+        sed_change (:obj:`ModelAttributeChange`): SED model change
+        smoldyn_change (:obj:`SimulationChange`): Smoldyn representation of the model change
+    '''
+    new_value = str(sed_change.new_value).strip()
+    new_line = smoldyn_change.command(new_value)
+    smoldyn_simulation_configuration.insert(0, new_line)
+
+
+def get_smoldyn_run_timecourse_args(sed_simulation):
+    ''' Get the Smoldyn representation of a SED uniform time course simulation
+
+    Args:
+        sed_simulation (:obj:`UniformTimeCourseSimulation`): SED uniform time course simulation
+
+    Returns:
+        :obj:`dict`: dictionary with keys ``start``, ``stop``, and ``dt`` that captures the Smoldyn
+            representation of the time course
+
+    Raises:
+        :obj:`NotImplementedError`: unsupported timecourse
+    '''
+    number_of_steps = (
+        (
+            sed_simulation.output_end_time - sed_simulation.initial_time
+        ) / (
+            sed_simulation.output_end_time - sed_simulation.output_start_time
+        ) * (
+            sed_simulation.number_of_steps
+        )
+    )
+    if (number_of_steps - int(number_of_steps)) > 1e-8:
+        msg = (
+            'Simulations must specify an integer number of steps, not {}.'
+            '\n  Initial time: {}'
+            '\n  Output start time: {}'
+            '\n  Output end time: {}'
+            '\n  Number of steps (output start to end time): {}'
+        ).format(
+            number_of_steps,
+            sed_simulation.initial_time,
+            sed_simulation.output_start_time,
+            sed_simulation.output_end_time,
+            sed_simulation.number_of_steps,
+        )
+        raise NotImplementedError(msg)
+
+    dt = (sed_simulation.output_end_time - sed_simulation.output_start_time) / sed_simulation.number_of_steps
+
+    return {
+        'start': sed_simulation.initial_time,
+        'stop': sed_simulation.output_end_time,
+        'dt': dt,
+    }
+
+
+def get_smoldyn_instance_attr_or_run_algorithm_parameter_arg(sed_algorithm_parameter_change):
+    ''' Get the Smoldyn representation of a SED uniform time course simulation
+
+    Args:
+        sed_algorithm_parameter_change (:obj:`AlgorithmParameterChange`): SED change to a parameter of an algorithm
+
+    Returns:
+        :obj:`dict`: dictionary with keys ``type``, ``name``, and ``value`` that captures the Smoldyn representation
+            of the algorithm parameter
+
+    Raises:
+        :obj:`ValueError`: unsupported algorithm parameter value
+        :obj:`NotImplementedError`: unsupported algorithm parameter
+    '''
+    parameter_props = KISAO_ALGORITHM_PARAMETERS_MAP.get(sed_algorithm_parameter_change.kisao_id, None)
+    if parameter_props:
+        if not validate_str_value(sed_algorithm_parameter_change.new_value, parameter_props['data_type']):
+            msg = '{} ({}) must be a {}, not `{}`.'.format(
+                parameter_props['name'], sed_algorithm_parameter_change.kisao_id,
+                parameter_props['data_type'].name, sed_algorithm_parameter_change.new_value,
+            )
+            raise ValueError(msg)
+        new_value = parse_value(sed_algorithm_parameter_change.new_value, parameter_props['data_type'])
+
+        return {
+            'type': parameter_props['type'],
+            'name': parameter_props['name'],
+            'value': new_value,
+        }
+
+    else:
+        msg = 'Algorithm parameter `{}` is not supported. The following parameters are supported:{}'.format(
+            sed_algorithm_parameter_change.kisao_id,
+            ''.join('\n  {}: {}'.format(kisao_id, parameter_props['name'])
+                    for kisao_id, parameter_props in KISAO_ALGORITHM_PARAMETERS_MAP.items())
+        )
+        raise NotImplementedError(msg)
+
+
+def add_smoldyn_output_file(configuration_dirname, smoldyn_simulation):
+    ''' Add an output file to a Smoldyn simulation
+
+    Args:
+        configuration_dirname (:obj:`str`): path to the parent directory of the Smoldyn configuration file for the simulation
+        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
+
+    Returns:
+        :obj:`SmoldynOutputFile`: output file
+    '''
+    fid, filename = tempfile.mkstemp(dir=configuration_dirname, suffix='.ssv')
+    os.close(fid)
+    name = os.path.relpath(filename, configuration_dirname)
+    smoldyn_simulation.setOutputFile(name, append=False)
+    smoldyn_simulation.setOutputPath('./')
+    return SmoldynOutputFile(name=name, filename=filename)
+
+
+def add_commands_to_smoldyn_output_file(simulation, output_file, commands):
+    ''' Add commands to a Smoldyn output file
+
+    Args:
+        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
+        smoldyn_output_file (:obj:`SmoldynOutputFile`): Smoldyn output file
+        commands (:obj:`list` of :obj`SmoldynCommand`): Smoldyn commands
+    '''
+    for command in commands:
+        simulation.addCommand(command.command + ' ' + output_file.name, command.type)
+
+
+def validate_variables(variables):
+    ''' Validate SED variables
+
+    =============================================================================================================================================  ===========================================================================================================================================  ===========================================
+    Smoldyn output file                                                                                                                            SED variable target                                                                                                                          Shape
+    =============================================================================================================================================  ===========================================================================================================================================  ===========================================
+    ``molcount``                                                                                                                                   ``molcount {species}``                                                                                                                       (numberOfSteps + 1,)
+    ``molcountspecies {species}({state})``                                                                                                         ``molcountspecies {species}({state})``                                                                                                       (numberOfSteps + 1,)
+    ``molcountspecieslist {species}({state})+``                                                                                                    ``molcountspecies {species}({state})``                                                                                                       (numberOfSteps + 1,)
+    ``molcountinbox {low-x} {hi-x}``                                                                                                               ``molcountinbox {species} {low-x} {hi-x}``                                                                                                   (numberOfSteps + 1,)
+    ``molcountinbox {low-x} {hi-x} {low-y} {hi-y}``                                                                                                ``molcountinbox {species} {low-x} {hi-x} {low-y} {hi-y}``                                                                                    (numberOfSteps + 1,)
+    ``molcountinbox {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z}``                                                                                 ``molcountinbox {species} {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z}``                                                                     (numberOfSteps + 1,)
+    ``molcountincmpt {compartment}``                                                                                                               ``molcountincmpt {species} {compartment}``                                                                                                   (numberOfSteps + 1,)
+    ``molcountincmpts {compartment}+``                                                                                                             ``molcountincmpt {species} {compartment}``                                                                                                   (numberOfSteps + 1,)
+    ``molcountincmpt2 {compartment} {state}``                                                                                                      ``molcountincmpt2 {species} {compartment} {state}``                                                                                          (numberOfSteps + 1,)
+    ``molcountonsurf {surface}``                                                                                                                   ``molcountonsurf {species} {surface}``                                                                                                       (numberOfSteps + 1,)
+    ``molcountspace {species}({state}) {axis} {low} {hi} {bins} 0``                                                                                ``molcountspace {species}({state}) {axis} {low} {hi} {bins}``                                                                                (numberOfSteps + 1, bins)
+    ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi} 0``                                                                     ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi}``                                                                     (numberOfSteps + 1, bins)
+    ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi} {low} {hi} 0``                                                          ``molcountspace {species}({state}) {axis} {low} {hi} {bins} {low} {hi} {low} {hi}``                                                          (numberOfSteps + 1, bins)
+    ``molcountspace2d {species}({state}) z {low-x} {hi-x} {bins-x} {low-y} {hi-y} {bins-y} 0``                                                     ``molcountspace2d {species}({state}) z {low-x} {hi-x} {bins-x} {low-y} {hi-y} {bins-y}``                                                     (numberOfSteps + 1, bins-x, bins-y)
+    ``molcountspace2d {species}({state}) {axis} {low-1} {hi-1} {bins-1} {low-2} {hi-2} {bins-2} {low-3} {hi-3} 0``                                 ``molcountspace2d {species}({state}) {axis} {low-1} {hi-1} {bins-1} {low-2} {hi-2} {bins-3} {low-3} {hi-3}``                                 (numberOfSteps + 1, bins-1, bins-2)
+    ``molcountspaceradial {species}({state}) {center-x} {radius} {bins} 0``                                                                        ``molcountspaceradial {species}({state}) {center-x} {radius} {bins}``                                                                        (numberOfSteps + 1, bins)
+    ``molcountspaceradial {species}({state}) {center-x} {center-y} {radius} {bins} 0``                                                             ``molcountspaceradial {species}({state}) {center-x} {center-y} {radius} {bins}``                                                             (numberOfSteps + 1, bins)
+    ``molcountspaceradial {species}({state}) {center-x} {center-y} {center-z} {radius} {bins} 0``                                                  ``molcountspaceradial {species}({state}) {center-x} {center-y} {center-z} {radius} {bins}``                                                  (numberOfSteps + 1, bins)
+    ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {pole-x} {pole-y} {radius-min} {radius-max} {bins} 0``                      ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {pole-x} {pole-y} {radius-min} {radius-max} {bins}``                      (numberOfSteps + 1, bins)
+    ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {center-z} {pole-x} {pole-y} {pole-z} {radius-min} {radius-max} {bins} 0``  ``molcountspacepolarangle {species}({state}) {center-x} {center-y} {center-z} {pole-x} {pole-y} {pole-z} {radius-min} {radius-max} {bins}``  (numberOfSteps + 1, bins)
+    ``radialdistribution {species-1}({state-1}) {species-2}({state-2}) {radius} {bins} 0``                                                         ``radialdistribution {species-1}({state-1}) {species-2}({state-2}) {radius} {bins}``                                                         (numberOfSteps + 1, bins)
+    ``radialdistribution2 {species-1}({state-1}) {species-2}({state-2}) {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z} {radius} {bins} 0``           ``radialdistribution2 {species-1}({state-1}) {species-2}({state-2}) {low-x} {hi-x} {low-y} {hi-y} {low-z} {hi-z} {radius} {bins}``           (numberOfSteps + 1, bins)
+    =============================================================================================================================================   ==========================================================================================================================================  ===========================================
+
+    Args:
+        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
+
+    Returns:
+        :obj:`dict`: dictionary that maps variable targets and symbols to Smoldyn output commands
+    '''
+    # TODO: support additional kinds of outputs
+
+    variable_output_cmd_map = {}
+
+    invalid_symbols = []
+    invalid_targets = []
+
+    for variable in variables:
+        if variable.symbol:
+            if variable.symbol == Symbol.time.value:
+                output_command_args = 'molcount'
+                include_header = True
+                shape = None
+                results_slicer = functools.partial(results_key_slicer, key='time')
+
+            else:
+                invalid_symbols.append('{}: {}'.format(variable.id, variable.symbol))
+                output_command_args = None
+                include_header = None
+
+        else:
+            output_command, _, output_args = re.sub(r' +', ' ', variable.target).partition(' ')
+
+            if output_command in ['molcount', 'molcountinbox', 'molcountincmpt', 'molcountincmpt2', 'molcountonsurf']:
+                species_name, _, output_args = output_args.partition(' ')
+                output_command_args = output_command + ' ' + output_args
+                include_header = True
+                shape = None
+                results_slicer = functools.partial(results_key_slicer, key=species_name)
+
+            elif output_command in ['molcountspecies']:
+                output_command_args = output_command + ' ' + output_args
+                include_header = False
+                shape = None
+                results_slicer = results_array_slicer
+
+            elif output_command in ['molcountspace', 'molcountspaceradial',
+                                    'molcountspacepolarangle', 'radialdistribution', 'radialdistribution2']:
+                output_command_args = output_command + ' ' + output_args + ' 0'
+                include_header = False
+                shape = None
+                results_slicer = results_matrix_slicer
+
+            elif output_command in ['molcountspace2d']:
+                output_command_args = output_command + ' ' + output_args + ' 0'
+                include_header = False
+                output_args_list = output_args.split(' ')
+                if len(output_args_list) == 8:
+                    shape = (int(output_args_list[-4]), int(output_args_list[-1]))
+                else:
+                    shape = (int(output_args_list[-6]), int(output_args_list[-3]))
+                results_slicer = None
+
+            else:
+                invalid_targets.append('{}: {}'.format(variable.id, variable.target))
+                output_command_args = None
+
+        if output_command_args is not None:
+            output_command_args = output_command_args.strip()
+            variable_output_cmd_map[(variable.target, variable.symbol)] = (output_command_args, include_header, shape, results_slicer)
+
+    if invalid_symbols:
+        msg = '{} symbols cannot be recorded:\n  {}\n\nThe following symbols can be recorded:\n  {}'.format(
+            len(invalid_symbols),
+            '\n  '.join(sorted(invalid_symbols)),
+            '\n  '.join(sorted([Symbol.time.value])),
+        )
+        raise ValueError(msg)
+
+    if invalid_targets:
+        valid_target_output_commands = [
+            'molcount',
+
+            'molcount', 'molcountinbox', 'molcountincmpt', 'molcountincmpt2', 'molcountonsurf',
+
+            'molcountspace', 'molcountspaceradial',
+            'molcountspacepolarangle', 'radialdistribution', 'radialdistribution2',
+
+            'molcountspace2d',
+        ]
+
+        msg = '{} targets cannot be recorded:\n  {}\n\nTargets are supported for the following output commands:\n  {}'.format(
+            len(invalid_targets),
+            '\n  '.join(sorted(invalid_targets)),
+            '\n  '.join(sorted(set(valid_target_output_commands))),
+        )
+        raise NotImplementedError(msg)
+
+    return variable_output_cmd_map
+
+
+def results_key_slicer(results, key):
+    """ Get the results for a key from a set of results
+
+    Args:
+        results (:obj:`pandas.DataFrame`): set of results
+
+    Returns:
+        :obj:`pandas.DataFrame`: results for a key
+    """
+    return results.get(key, None)
+
+
+def results_array_slicer(results):
+    """ Extract an array of results from a matrix of time and results
+
+    Args:
+        results (:obj:`pandas.DataFrame`): matrix of time and results
+
+    Returns:
+        :obj:`pandas.DataFrame`: results
+    """
+    return results.iloc[:, 1]
+
+
+def results_matrix_slicer(results):
+    """ Extract a matrix array of results from a matrix of time and results
+
+    Args:
+        results (:obj:`pandas.DataFrame`): matrix of time and results
+
+    Returns:
+        :obj:`pandas.DataFrame`: results
+    """
+    return results.iloc[:, 1:]
+
+
+def add_smoldyn_output_files_for_sed_variables(configuration_dirname, variables, variable_output_cmd_map, smoldyn_simulation):
+    ''' Add Smoldyn output files for capturing each SED variable
+
+    Args:
+        configuration_dirname (:obj:`str`): path to the parent directory of the Smoldyn configuration file for the simulation
+        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
+        variable_output_cmd_map (:obj:`dict`): dictionary that maps variable targets and symbols to Smoldyn output commands
+        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
+
+    Returns:
+        :obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`: Smoldyn output files
+    '''
+    smoldyn_output_files = {}
+
+    output_cmds = set()
+    for variable in variables:
+        output_cmds.add(variable_output_cmd_map[(variable.target, variable.symbol)])
+
+    for command, include_header, _, _ in output_cmds:
+        add_smoldyn_output_file_for_output(configuration_dirname, smoldyn_simulation,
+                                           command, include_header,
+                                           smoldyn_output_files)
+    # return output files
+    return smoldyn_output_files
+
+
+def add_smoldyn_output_file_for_output(configuration_dirname, smoldyn_simulation,
+                                       smoldyn_output_command, include_header, smoldyn_output_files):
+    ''' Add a Smoldyn output file for molecule counts
+
+    Args:
+        configuration_dirname (:obj:`str`): path to the parent directory of the Smoldyn configuration file for the simulation
+        smoldyn_simulation (:obj:`smoldyn.Simulation`): Smoldyn simulation
+        smoldyn_output_command (:obj:`str`): Smoldyn output command (e.g., ``molcount``)
+        include_header (:obj:`bool`): whether to include a header
+        smoldyn_output_files (:obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`): Smoldyn output files
+    '''
+    smoldyn_output_files[smoldyn_output_command] = add_smoldyn_output_file(configuration_dirname, smoldyn_simulation)
+
+    commands = []
+    if include_header:
+        commands.append(SmoldynCommand('molcountheader', 'B'))
+    commands.append(SmoldynCommand(smoldyn_output_command, 'E'))
+
+    add_commands_to_smoldyn_output_file(
+        smoldyn_simulation,
+        smoldyn_output_files[smoldyn_output_command],
+        commands,
+    )
+
+
+def get_variable_results(number_of_steps, variables, variable_output_cmd_map, smoldyn_output_files):
+    ''' Get the result of each SED variable
+
+    Args:
+        number_of_steps (:obj:`int`): number of steps
+        variables (:obj:`list` of :obj:`Variable`): variables that should be recorded
+        variable_output_cmd_map (:obj:`dict`): dictionary that maps variable targets and symbols to Smoldyn output commands
+        smoldyn_output_files (:obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`): Smoldyn output files
+
+    Returns:
+        :obj:`VariableResults`: result of each SED variable
+
+    Raises:
+        :obj:`ValueError`: unsupported results
+    '''
+    smoldyn_results = {}
+
+    missing_variables = []
+
+    variable_results = VariableResults()
+    for variable in variables:
+        output_command_args, _, shape, results_slicer = variable_output_cmd_map[(variable.target, variable.symbol)]
+        variable_result = get_smoldyn_output(output_command_args, True, shape, smoldyn_output_files, smoldyn_results)
+        if results_slicer:
+            variable_result = results_slicer(variable_result)
+
+        if variable_result is None:
+            missing_variables.append('{}: {}: {}'.format(variable.id, 'target', variable.target))
+        else:
+            if variable_result.ndim == 1:
+                variable_results[variable.id] = variable_result.to_numpy()[-(number_of_steps + 1):, ]
+            elif variable_result.ndim == 2:
+                variable_results[variable.id] = variable_result.to_numpy()[-(number_of_steps + 1):, :]
+            else:
+                variable_results[variable.id] = variable_result[-(number_of_steps + 1):, :, :]
+
+    if missing_variables:
+        msg = '{} variables could not be recorded:\n  {}'.format(
+            len(missing_variables),
+            '\n  '.join(missing_variables),
+        )
+        raise ValueError(msg)
+
+    return variable_results
+
+
+def get_smoldyn_output(smoldyn_output_command, has_header, three_d_shape, smoldyn_output_files, smoldyn_results):
+    ''' Get the simulated count of each molecule
+
+    Args:
+        smoldyn_output_command (:obj:`str`): Smoldyn output command (e.g., ``molcount``)
+        has_header (:obj:`bool`): whether to include a header
+        three_d_shape (:obj:`tuple` of :obj:`int`): dimensions of the output
+        smoldyn_output_files (:obj:`dict` of :obj:`str` => :obj:`SmoldynOutputFile`): Smoldyn output files
+        smoldyn_results (:obj:`dict`)
+
+    Returns:
+        :obj:`pandas.DataFrame` or :obj:`numpy.ndarray`: results
+    '''
+    smoldyn_output_command = smoldyn_output_command.strip()
+    if smoldyn_output_command not in smoldyn_results:
+        smoldyn_output_file = smoldyn_output_files[smoldyn_output_command]
+        if three_d_shape:
+            with open(smoldyn_output_file.filename, 'r') as file:
+                data_list = []
+
+                i_line = 0
+                for line in file:
+                    if i_line % (three_d_shape[1] + 1) == 0:
+                        time_point_data = []
+                    else:
+                        profile = [int(el) for el in line.split(' ')]
+                        time_point_data.append(profile)
+
+                        if i_line % (three_d_shape[1] + 1) == three_d_shape[1]:
+                            data_list.append(time_point_data)
+
+                    i_line += 1
+
+            smoldyn_results[smoldyn_output_command] = numpy.array(data_list).transpose((0, 2, 1))
+
+        else:
+            smoldyn_results[smoldyn_output_command] = pandas.read_csv(smoldyn_output_file.filename, sep=' ')
+
+    return smoldyn_results[smoldyn_output_command]
```

## smoldyn/biosimulators/_version.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from smoldyn import __version__  # noqa: F401
+from smoldyn import __version__  # noqa: F401
```

## smoldyn/biosimulators/__init__.py

 * *Ordering differences only*

```diff
@@ -1,21 +1,21 @@
-from ._version import __version__
-from .combine import preprocess_sed_task, exec_sed_task, exec_sed_doc, exec_sedml_docs_in_combine_archive  # noqa: F401
-import smoldyn
-
-__all__ = [
-    '__version__',
-    'get_simulator_version',
-    'preprocess_sed_task',
-    'exec_sed_task',
-    'exec_sed_doc',
-    'exec_sedml_docs_in_combine_archive',
-]
-
-
-def get_simulator_version():
-    """ Get the version of Smoldyn
-
-    Returns:
-        :obj:`str`: version
-    """
-    return smoldyn.__version__
+from ._version import __version__
+from .combine import preprocess_sed_task, exec_sed_task, exec_sed_doc, exec_sedml_docs_in_combine_archive  # noqa: F401
+import smoldyn
+
+__all__ = [
+    '__version__',
+    'get_simulator_version',
+    'preprocess_sed_task',
+    'exec_sed_task',
+    'exec_sed_doc',
+    'exec_sedml_docs_in_combine_archive',
+]
+
+
+def get_simulator_version():
+    """ Get the version of Smoldyn
+
+    Returns:
+        :obj:`str`: version
+    """
+    return smoldyn.__version__
```

## smoldyn/biosimulators/data_model.py

 * *Ordering differences only*

```diff
@@ -1,169 +1,169 @@
-''' Data model for representing configurations for Smoldyn simulations for use with SED-ML
-'''
-
-from biosimulators_utils.data_model import ValueType
-import enum
-import types  # noqa: F401
-
-__author__ = 'Jonathan Karr'
-__email__ = 'karr@mssm.edu'
-
-__all__ = [
-    'Simulation',
-    'SimulationInstruction',
-    'SmoldynCommand',
-    'SmoldynOutputFile',
-    'SimulationChange',
-    'SimulationChangeExecution',
-    'AlgorithmParameterType',
-    'KISAO_ALGORITHMS_MAP',
-    'KISAO_ALGORITHM_PARAMETERS_MAP',
-]
-
-
-class Simulation(object):
-    """ Configuration of a simulation
-
-    Attributes:
-        species (:obj:`list` of :obj:`str`): names of species
-        compartments (:obj:`list` of :obj:`str`): names of compartments
-        surfaces (:obj:`list` of :obj:`str`): names of surfaces
-        instructions (:obj:`list` of :obj:`SimulationInstruction`): instructions
-    """
-
-    def __init__(self, species=None, compartments=None, surfaces=None, instructions=None):
-        """
-        Args:
-            species (:obj:`list` of :obj:`str`, optional): names of species
-            compartments (:obj:`list` of :obj:`str`, optional): names of compartments
-            surfaces (:obj:`list` of :obj:`str`, optional): names of surfaces
-            instructions (:obj:`list` of :obj:`SimulationInstruction`, optional): instructions
-        """
-        self.species = species or []
-        self.compartments = compartments or []
-        self.surfaces = surfaces or []
-        self.instructions = instructions or []
-
-
-class SimulationInstruction(object):
-    """ Configuration of a simulation
-
-    Attributes:
-        macro (:obj:`str`): Smoldyn macro
-        arguments (:obj:`str`): arguments of the Smoldyn macro
-        id (:obj:`str`): unique id of the instruction
-        description (:obj:`str`): human-readable description of the instruction
-        comment (:obj:`str`): comment about the instruction
-    """
-
-    def __init__(self, macro, arguments, id=None, description=None, comment=None):
-        """
-        Args:
-            macro (:obj:`str`): Smoldyn macro
-            arguments (:obj:`str`): arguments of the Smoldyn macro
-            id (:obj:`str`, optional): unique id of the instruction
-            description (:obj:`str`, optional): human-readable description of the instruction
-            comment (:obj:`str`, optional): comment about the instruction
-        """
-        self.macro = macro
-        self.arguments = arguments
-        self.id = id
-        self.description = description
-        self.comment = comment
-
-    def is_equal(self, other):
-        return (self.__class__ == other.__class__
-                and self.macro == other.macro
-                and self.arguments == other.arguments
-                and self.id == other.id
-                and self.description == other.description
-                and self.comment == other.comment
-                )
-
-
-class SmoldynCommand(object):
-    ''' A Smoldyn command
-
-    Attributes:
-        command (:obj:`str`): command (e.g., ``molcount``)
-        type (:obj:`str`): command type (e.g., ``E``)
-    '''
-
-    def __init__(self, command, type):
-        '''
-        Args:
-            command (:obj:`str`): command (e.g., ``molcount``)
-            type (:obj:`str`): command type (e.g., ``E``)
-        '''
-        self.command = command
-        self.type = type
-
-
-class SmoldynOutputFile(object):
-    ''' A Smoldyn output file
-
-    Attributes:
-        name (:obj:`str`): name
-        filename (:obj:`str`): path to the file
-    '''
-
-    def __init__(self, name, filename):
-        '''
-        Args:
-            name (:obj:`str`): name
-            filename (:obj:`str`): path to the file
-        '''
-        self.name = name
-        self.filename = filename
-
-
-class SimulationChange(object):
-    ''' A change to a Smoldyn simulation
-
-    Attributes:
-        command (:obj:`types.FunctionType`): function for generating a Smoldyn configuration command for a new value
-        execution (:obj:`SimulationChangeExecution`): operation when change should be executed
-    '''
-
-    def __init__(self, command, execution):
-        '''
-        Args:
-            command (:obj:`types.FunctionType`): function for generating a Smoldyn configuration command for a new value
-        execution (:obj:`SimulationChangeExecution`): operation when change should be executed
-        '''
-        self.command = command
-        self.execution = execution
-
-
-class SimulationChangeExecution(str, enum.Enum):
-    """ Operation when a simulation change should be executed """
-    preprocessing = 'preprocessing'
-    simulation = 'simulation'
-
-
-class AlgorithmParameterType(str, enum.Enum):
-    ''' Type of algorithm parameter '''
-    run_argument = 'run_argument'
-    instance_attribute = 'instance_attribute'
-
-
-KISAO_ALGORITHMS_MAP = {
-    'KISAO_0000057': {
-        'name': 'Brownian diffusion Smoluchowski method',
-    }
-}
-
-KISAO_ALGORITHM_PARAMETERS_MAP = {
-    'KISAO_0000254': {
-        'name': 'accuracy',
-        'type': AlgorithmParameterType.run_argument,
-        'data_type': ValueType.float,
-        'default': 10.,
-    },
-    'KISAO_0000488': {
-        'name': 'setRandomSeed',
-        'type': AlgorithmParameterType.instance_attribute,
-        'data_type': ValueType.integer,
-        'default': None,
-    },
-}
+''' Data model for representing configurations for Smoldyn simulations for use with SED-ML
+'''
+
+from biosimulators_utils.data_model import ValueType
+import enum
+import types  # noqa: F401
+
+__author__ = 'Jonathan Karr'
+__email__ = 'karr@mssm.edu'
+
+__all__ = [
+    'Simulation',
+    'SimulationInstruction',
+    'SmoldynCommand',
+    'SmoldynOutputFile',
+    'SimulationChange',
+    'SimulationChangeExecution',
+    'AlgorithmParameterType',
+    'KISAO_ALGORITHMS_MAP',
+    'KISAO_ALGORITHM_PARAMETERS_MAP',
+]
+
+
+class Simulation(object):
+    """ Configuration of a simulation
+
+    Attributes:
+        species (:obj:`list` of :obj:`str`): names of species
+        compartments (:obj:`list` of :obj:`str`): names of compartments
+        surfaces (:obj:`list` of :obj:`str`): names of surfaces
+        instructions (:obj:`list` of :obj:`SimulationInstruction`): instructions
+    """
+
+    def __init__(self, species=None, compartments=None, surfaces=None, instructions=None):
+        """
+        Args:
+            species (:obj:`list` of :obj:`str`, optional): names of species
+            compartments (:obj:`list` of :obj:`str`, optional): names of compartments
+            surfaces (:obj:`list` of :obj:`str`, optional): names of surfaces
+            instructions (:obj:`list` of :obj:`SimulationInstruction`, optional): instructions
+        """
+        self.species = species or []
+        self.compartments = compartments or []
+        self.surfaces = surfaces or []
+        self.instructions = instructions or []
+
+
+class SimulationInstruction(object):
+    """ Configuration of a simulation
+
+    Attributes:
+        macro (:obj:`str`): Smoldyn macro
+        arguments (:obj:`str`): arguments of the Smoldyn macro
+        id (:obj:`str`): unique id of the instruction
+        description (:obj:`str`): human-readable description of the instruction
+        comment (:obj:`str`): comment about the instruction
+    """
+
+    def __init__(self, macro, arguments, id=None, description=None, comment=None):
+        """
+        Args:
+            macro (:obj:`str`): Smoldyn macro
+            arguments (:obj:`str`): arguments of the Smoldyn macro
+            id (:obj:`str`, optional): unique id of the instruction
+            description (:obj:`str`, optional): human-readable description of the instruction
+            comment (:obj:`str`, optional): comment about the instruction
+        """
+        self.macro = macro
+        self.arguments = arguments
+        self.id = id
+        self.description = description
+        self.comment = comment
+
+    def is_equal(self, other):
+        return (self.__class__ == other.__class__
+                and self.macro == other.macro
+                and self.arguments == other.arguments
+                and self.id == other.id
+                and self.description == other.description
+                and self.comment == other.comment
+                )
+
+
+class SmoldynCommand(object):
+    ''' A Smoldyn command
+
+    Attributes:
+        command (:obj:`str`): command (e.g., ``molcount``)
+        type (:obj:`str`): command type (e.g., ``E``)
+    '''
+
+    def __init__(self, command, type):
+        '''
+        Args:
+            command (:obj:`str`): command (e.g., ``molcount``)
+            type (:obj:`str`): command type (e.g., ``E``)
+        '''
+        self.command = command
+        self.type = type
+
+
+class SmoldynOutputFile(object):
+    ''' A Smoldyn output file
+
+    Attributes:
+        name (:obj:`str`): name
+        filename (:obj:`str`): path to the file
+    '''
+
+    def __init__(self, name, filename):
+        '''
+        Args:
+            name (:obj:`str`): name
+            filename (:obj:`str`): path to the file
+        '''
+        self.name = name
+        self.filename = filename
+
+
+class SimulationChange(object):
+    ''' A change to a Smoldyn simulation
+
+    Attributes:
+        command (:obj:`types.FunctionType`): function for generating a Smoldyn configuration command for a new value
+        execution (:obj:`SimulationChangeExecution`): operation when change should be executed
+    '''
+
+    def __init__(self, command, execution):
+        '''
+        Args:
+            command (:obj:`types.FunctionType`): function for generating a Smoldyn configuration command for a new value
+        execution (:obj:`SimulationChangeExecution`): operation when change should be executed
+        '''
+        self.command = command
+        self.execution = execution
+
+
+class SimulationChangeExecution(str, enum.Enum):
+    """ Operation when a simulation change should be executed """
+    preprocessing = 'preprocessing'
+    simulation = 'simulation'
+
+
+class AlgorithmParameterType(str, enum.Enum):
+    ''' Type of algorithm parameter '''
+    run_argument = 'run_argument'
+    instance_attribute = 'instance_attribute'
+
+
+KISAO_ALGORITHMS_MAP = {
+    'KISAO_0000057': {
+        'name': 'Brownian diffusion Smoluchowski method',
+    }
+}
+
+KISAO_ALGORITHM_PARAMETERS_MAP = {
+    'KISAO_0000254': {
+        'name': 'accuracy',
+        'type': AlgorithmParameterType.run_argument,
+        'data_type': ValueType.float,
+        'default': 10.,
+    },
+    'KISAO_0000488': {
+        'name': 'setRandomSeed',
+        'type': AlgorithmParameterType.instance_attribute,
+        'data_type': ValueType.integer,
+        'default': None,
+    },
+}
```

## smoldyn/biosimulators/utils.py

 * *Ordering differences only*

```diff
@@ -1,349 +1,349 @@
-''' Methods for parsing configurations of Smoldyn simulations for use with SED-ML
-'''
-
-__author__ = 'Jonathan Karr'
-__email__ = 'karr@mssm.edu'
-
-__all__ = [
-    'read_simulation',
-]
-
-from .data_model import Simulation, SimulationInstruction
-import re
-
-
-def read_simulation(filename):
-    """ Read the configuration for a Smoldyn simulation
-
-    Args:
-        filename (:obj:`str`): path to a configuration for a Smoldyn simulation
-
-    Returns:
-        :obj:`Simulation`: data structure which represents the configuration of the Smoldyn simulation
-    """
-    sim = Simulation()
-    param_group_counts = {}
-    with open(filename, 'r') as file:
-        for line in file:
-            # separate comments
-            line, _, comment = line.partition('#')
-            line = line.strip()
-            comment = comment.strip()
-
-            # remove consecutive spaces
-            line = re.sub(' +', ' ', line)
-
-            _read_simulation_line(line, param_group_counts, sim)
-
-            if re.match(r'^end_file( |$)', line):
-                break
-
-    return sim
-
-
-def _read_simulation_line(line, macro_counts, sim):
-    """ Parse a line of a configuration of a Smoldyn simulation
-
-    Args:
-        line (:obj:`str`): line of a configuration of a Smoldyn simulation
-        macro_counts (:obj:`dict`): dictionary used to count instances of the same macro
-        sim (:obj:`Simulation`): data structure which represents the configuration of the Smoldyn simulation
-    """
-    if line.startswith('species '):
-        sim.species.extend(line.split(' ')[1:])
-
-    elif line.startswith('start_compartment '):
-        sim.compartments.append(line.partition(' ')[2])
-
-    elif line.startswith('start_surface '):
-        sim.surfaces.append(line.partition(' ')[2])
-
-    for pattern in CONFIG_DECLARATION_PATTERNS:
-        match = re.match(pattern['regex'], line)
-        if match:
-            if pattern.get('macro', None):
-                group = pattern['macro']['group'](match)
-                if group not in macro_counts:
-                    macro_counts[group] = -1
-                macro_counts[group] += 1
-                i_group = macro_counts[group]
-
-                sim.instructions.append(SimulationInstruction(
-                    id=pattern['macro']['id'](match, i_group),
-                    description=pattern['macro']['description'](match, i_group),
-                    macro=pattern['macro']['macro'](match),
-                    arguments=pattern['macro']['arguments'](match),
-                ))
-
-
-CONFIG_DECLARATION_PATTERNS = [
-    {
-        'regex': r'^(dim) (.*?)$',
-        'macro': {
-            'group': lambda match: 'number_dimensions',
-            'id': lambda match, i_group: 'number_dimensions',
-            'description': lambda match, i_group: 'Number of dimensions',
-            'macro': lambda match: match.group(1),
-            'arguments': lambda match: match.group(2),
-        }
-    },
-    {
-        'regex': r'^low_wall ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'low_wall_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'low_{}_wall_{}'.format(match.group(1), i_group + 1),
-            'description': lambda match, i_group: 'Low {} wall {}'.format(match.group(1), i_group + 1),
-            'macro': lambda match: 'low_wall {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^high_wall ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'high_wall_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'high_{}_wall_{}'.format(match.group(1), i_group + 1),
-            'description': lambda match, i_group: 'High {} wall {}'.format(match.group(1), i_group + 1),
-            'macro': lambda match: 'high_wall {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^boundaries ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'boundaries_{}'.format(match.group(1)),
-            'id': lambda match, i_group: '{}_boundary'.format(match.group(1)),
-            'description': lambda match, i_group: '{} boundary'.format(match.group(1).upper()),
-            'macro': lambda match: 'boundaries {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^define ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'define_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'value_parameter_{}'.format(match.group(1)),
-            'description': lambda match, i_group: 'Value of parameter "{}"'.format(match.group(1)),
-            'macro': lambda match: 'define {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^difc ([^ \(\)]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difc_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'diffusion_coefficient_species_{}'.format(match.group(1)),
-            'description': lambda match, i_group: 'Diffusion coefficient of species "{}"'.format(match.group(1)),
-            'macro': lambda match: 'difc {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^difc ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difc_{}_{}'.format(match.group(1), match.group(2)),
-            'id': lambda match, i_group: 'diffusion_coefficient_species_{}_state_{}'.format(match.group(1), match.group(2)),
-            'description': lambda match, i_group: 'Diffusion coefficient of species "{}" in state "{}"'.format(match.group(1), match.group(2)),
-            'macro': lambda match: 'difc {}({})'.format(match.group(1), match.group(2)),
-            'arguments': lambda match: match.group(3),
-        },
-    },
-    {
-        'regex': r'^difc_rule ([^ \(\)]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difc_rule_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'diffusion_coefficient_rule_species_{}'.format(re.sub('[^a-zA-Z0-9_]', '_', match.group(1))),
-            'description': lambda match, i_group: 'Diffusion coefficient rule for species "{}"'.format(match.group(1)),
-            'macro': lambda match: 'difc_rule {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^difc_rule ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difc_rule_{}_{}'.format(
-                match.group(1), match.group(2)),
-            'id': lambda match, i_group: 'diffusion_coefficient_rule_species_{}_state_{}'.format(
-                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2)),
-            'description': lambda match, i_group: 'Diffusion coefficient rule for species "{}" in state "{}"'.format(
-                match.group(1), match.group(2)),
-            'macro': lambda match: 'difc_rule {}({})'.format(
-                match.group(1), match.group(2)),
-            'arguments': lambda match: match.group(3),
-        },
-    },
-    {
-        'regex': r'^difm ([^ \(\)]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difm_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'membrane_diffusion_coefficient_species_{}'.format(match.group(1)),
-            'description': lambda match, i_group: 'Membrane diffusion coefficient of species "{}"'.format(match.group(1)),
-            'macro': lambda match: 'difm {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^difm ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difm_{}_{}'.format(match.group(1), match.group(2)),
-            'id': lambda match, i_group: 'membrane_diffusion_coefficient_species_{}_state_{}'.format(
-                match.group(1), match.group(2)),
-            'description': lambda match, i_group: 'Membrane diffusion coefficient of species "{}" in state "{}"'.format(
-                match.group(1), match.group(2)),
-            'macro': lambda match: 'difm {}({})'.format(match.group(1), match.group(2)),
-            'arguments': lambda match: match.group(3),
-        },
-    },
-    {
-        'regex': r'^difm_rule ([^ \(\)]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difm_rule_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'membrane_diffusion_coefficient_rule_species_{}'.format(
-                re.sub('[^a-zA-Z0-9_]', '_', match.group(1))),
-            'description': lambda match, i_group: 'Membrane diffusion coefficient rule for species "{}"'.format(match.group(1)),
-            'macro': lambda match: 'difm_rule {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^difm_rule ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
-        'macro': {
-            'group': lambda match: 'difm_rule_{}_{}'.format(match.group(1), match.group(2)),
-            'id': lambda match, i_group: 'membrane_diffusion_coefficient_rule_species_{}_state_{}'.format(
-                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2)),
-            'description': lambda match, i_group: 'Membrane diffusion coefficient rule for species "{}" in state "{}"'.format(
-                match.group(1), match.group(2)),
-            'macro': lambda match: 'difm_rule {}({})'.format(match.group(1), match.group(2)),
-            'arguments': lambda match: match.group(3),
-        },
-    },
-    {
-        'regex': r'^drift ([^ \(\)]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'drift_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'drift_species_{}'.format(match.group(1)),
-            'description': lambda match, i_group: 'Drift of species "{}"'.format(match.group(1)),
-            'macro': lambda match: 'drift {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^drift ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
-        'macro': {
-            'group': lambda match: 'drift_{}_{}'.format(match.group(1), match.group(2)),
-            'id': lambda match, i_group: 'drift_species_{}_state_{}'.format(
-                match.group(1), match.group(2)),
-            'description': lambda match, i_group: 'Drift of species "{}" in state "{}"'.format(
-                match.group(1), match.group(2)),
-            'macro': lambda match: 'drift {}({})'.format(match.group(1), match.group(2)),
-            'arguments': lambda match: match.group(3),
-        },
-    },
-    {
-        'regex': r'^drift_rule ([^ \(\)]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'drift_rule_{}'.format(match.group(1)),
-            'id': lambda match, i_group: 'drift_rule_species_{}'.format(re.sub('[^a-zA-Z0-9_]', '_', match.group(1))),
-            'description': lambda match, i_group: 'Drift rule for species "{}"'.format(match.group(1)),
-            'macro': lambda match: 'drift_rule {}'.format(match.group(1)),
-            'arguments': lambda match: match.group(2),
-        },
-    },
-    {
-        'regex': r'^drift_rule ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
-        'macro': {
-            'group': lambda match: 'drift_rule_{}_{}'.format(match.group(1), match.group(2)),
-            'id': lambda match, i_group: 'drift_rule_species_{}_state_{}'.format(
-                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2)),
-            'description': lambda match, i_group: 'Drift rule for species "{}" in state "{}"'.format(
-                match.group(1), match.group(2)),
-            'macro': lambda match: 'drift_rule {}({})'.format(match.group(1), match.group(2)),
-            'arguments': lambda match: match.group(3),
-        },
-    },
-    {
-        'regex': r'^surface_drift ([^ \(\)]+) ([^ ]+) ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'surface_drift_{}_{}_{}'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'id': lambda match, i_group: 'surface_drift_species_{}_surface_{}_shape_{}'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'description': lambda match, i_group: 'Surface drift of species "{}" on surface "{}" with panel shape "{}"'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'macro': lambda match: 'surface_drift {} {} {}'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'arguments': lambda match: match.group(4),
-        },
-    },
-    {
-        'regex': r'^surface_drift ([^ \(\)]+)\(([^ \(\)]+)\) ([^ ]+) ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'surface_drift_{}_{}_{}_{}'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'id': lambda match, i_group: 'surface_drift_species_{}_state_{}_surface_{}_shape_{}'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'description': lambda match, i_group: 'Surface drift of species "{}" in state "{}" on surface "{}" with panel shape "{}"'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'macro': lambda match: 'surface_drift {}({}) {} {}'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'arguments': lambda match: match.group(5),
-        },
-    },
-    {
-        'regex': r'^surface_drift_rule ([^ \(\)]+) ([^ ]+) ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'surface_drift_rule_{}_{}_{}'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'id': lambda match, i_group: 'surface_drift_rule_species_{}_surface_{}_panel_{}'.format(
-                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2), match.group(3)),
-            'description': lambda match, i_group: 'Surface drift rule for species "{}" on surface "{}" of panel shape "{}"'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'macro': lambda match: 'surface_drift_rule {} {} {}'.format(
-                match.group(1), match.group(2), match.group(3)),
-            'arguments': lambda match: match.group(4),
-        },
-    },
-    {
-        'regex': r'^surface_drift_rule ([^ \(\)]+)\(([^ \(\)]+)\) ([^ ]+) ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'surface_drift_rule_{}_{}_{}_{}'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'id': lambda match, i_group: 'surface_drift_rule_species_{}_state_{}_surface_{}_panel_{}'.format(
-                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2), match.group(3), match.group(4)),
-            'description': lambda match, i_group: 'Surface drift rule for species "{}" in state "{}" on surface "{}" of panel shape "{}"'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'macro': lambda match: 'surface_drift_rule {}({}) {} {}'.format(
-                match.group(1), match.group(2), match.group(3), match.group(4)),
-            'arguments': lambda match: match.group(5),
-        },
-    },
-    {
-        'regex': r'^mol ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'mol_{}'.format(match.group(2)),
-            'id': lambda match, i_group: 'initial_count_species_{}'.format(re.sub(r'[^a-zA-Z0-9_]', '_', match.group(2))),
-            'description': lambda match, i_group: 'Initial count of species "{}"'.format(match.group(2)),
-            'macro': lambda match: 'mol {}'.format(match.group(2)),
-            'arguments': lambda match: match.group(1),
-        },
-    },
-    {
-        'regex': r'^compartment_mol ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'compartment_mol_{}'.format(match.group(2)),
-            'id': lambda match, i_group: 'initial_count_species_{}'.format(re.sub(r'[^a-zA-Z0-9_]', '_', match.group(2))),
-            'description': lambda match, i_group: 'Initial count of species "{}"'.format(match.group(2)),
-            'macro': lambda match: 'compartment_mol {}'.format(match.group(2)),
-            'arguments': lambda match: match.group(1),
-        },
-    },
-    {
-        'regex': r'^surface_mol ([^ ]+) (.*?)$',
-        'macro': {
-            'group': lambda match: 'surface_mol_{}'.format(match.group(2)),
-            'id': lambda match, i_group: 'initial_count_species_{}'.format(re.sub(r'[^a-zA-Z0-9_]', '_', match.group(2))),
-            'description': lambda match, i_group: 'Initial count of species "{}"'.format(match.group(2)),
-            'macro': lambda match: 'surface_mol {}'.format(match.group(2)),
-            'arguments': lambda match: match.group(1),
-        },
-    },
-]
+''' Methods for parsing configurations of Smoldyn simulations for use with SED-ML
+'''
+
+__author__ = 'Jonathan Karr'
+__email__ = 'karr@mssm.edu'
+
+__all__ = [
+    'read_simulation',
+]
+
+from .data_model import Simulation, SimulationInstruction
+import re
+
+
+def read_simulation(filename):
+    """ Read the configuration for a Smoldyn simulation
+
+    Args:
+        filename (:obj:`str`): path to a configuration for a Smoldyn simulation
+
+    Returns:
+        :obj:`Simulation`: data structure which represents the configuration of the Smoldyn simulation
+    """
+    sim = Simulation()
+    param_group_counts = {}
+    with open(filename, 'r') as file:
+        for line in file:
+            # separate comments
+            line, _, comment = line.partition('#')
+            line = line.strip()
+            comment = comment.strip()
+
+            # remove consecutive spaces
+            line = re.sub(' +', ' ', line)
+
+            _read_simulation_line(line, param_group_counts, sim)
+
+            if re.match(r'^end_file( |$)', line):
+                break
+
+    return sim
+
+
+def _read_simulation_line(line, macro_counts, sim):
+    """ Parse a line of a configuration of a Smoldyn simulation
+
+    Args:
+        line (:obj:`str`): line of a configuration of a Smoldyn simulation
+        macro_counts (:obj:`dict`): dictionary used to count instances of the same macro
+        sim (:obj:`Simulation`): data structure which represents the configuration of the Smoldyn simulation
+    """
+    if line.startswith('species '):
+        sim.species.extend(line.split(' ')[1:])
+
+    elif line.startswith('start_compartment '):
+        sim.compartments.append(line.partition(' ')[2])
+
+    elif line.startswith('start_surface '):
+        sim.surfaces.append(line.partition(' ')[2])
+
+    for pattern in CONFIG_DECLARATION_PATTERNS:
+        match = re.match(pattern['regex'], line)
+        if match:
+            if pattern.get('macro', None):
+                group = pattern['macro']['group'](match)
+                if group not in macro_counts:
+                    macro_counts[group] = -1
+                macro_counts[group] += 1
+                i_group = macro_counts[group]
+
+                sim.instructions.append(SimulationInstruction(
+                    id=pattern['macro']['id'](match, i_group),
+                    description=pattern['macro']['description'](match, i_group),
+                    macro=pattern['macro']['macro'](match),
+                    arguments=pattern['macro']['arguments'](match),
+                ))
+
+
+CONFIG_DECLARATION_PATTERNS = [
+    {
+        'regex': r'^(dim) (.*?)$',
+        'macro': {
+            'group': lambda match: 'number_dimensions',
+            'id': lambda match, i_group: 'number_dimensions',
+            'description': lambda match, i_group: 'Number of dimensions',
+            'macro': lambda match: match.group(1),
+            'arguments': lambda match: match.group(2),
+        }
+    },
+    {
+        'regex': r'^low_wall ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'low_wall_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'low_{}_wall_{}'.format(match.group(1), i_group + 1),
+            'description': lambda match, i_group: 'Low {} wall {}'.format(match.group(1), i_group + 1),
+            'macro': lambda match: 'low_wall {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^high_wall ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'high_wall_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'high_{}_wall_{}'.format(match.group(1), i_group + 1),
+            'description': lambda match, i_group: 'High {} wall {}'.format(match.group(1), i_group + 1),
+            'macro': lambda match: 'high_wall {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^boundaries ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'boundaries_{}'.format(match.group(1)),
+            'id': lambda match, i_group: '{}_boundary'.format(match.group(1)),
+            'description': lambda match, i_group: '{} boundary'.format(match.group(1).upper()),
+            'macro': lambda match: 'boundaries {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^define ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'define_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'value_parameter_{}'.format(match.group(1)),
+            'description': lambda match, i_group: 'Value of parameter "{}"'.format(match.group(1)),
+            'macro': lambda match: 'define {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^difc ([^ \(\)]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difc_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'diffusion_coefficient_species_{}'.format(match.group(1)),
+            'description': lambda match, i_group: 'Diffusion coefficient of species "{}"'.format(match.group(1)),
+            'macro': lambda match: 'difc {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^difc ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difc_{}_{}'.format(match.group(1), match.group(2)),
+            'id': lambda match, i_group: 'diffusion_coefficient_species_{}_state_{}'.format(match.group(1), match.group(2)),
+            'description': lambda match, i_group: 'Diffusion coefficient of species "{}" in state "{}"'.format(match.group(1), match.group(2)),
+            'macro': lambda match: 'difc {}({})'.format(match.group(1), match.group(2)),
+            'arguments': lambda match: match.group(3),
+        },
+    },
+    {
+        'regex': r'^difc_rule ([^ \(\)]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difc_rule_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'diffusion_coefficient_rule_species_{}'.format(re.sub('[^a-zA-Z0-9_]', '_', match.group(1))),
+            'description': lambda match, i_group: 'Diffusion coefficient rule for species "{}"'.format(match.group(1)),
+            'macro': lambda match: 'difc_rule {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^difc_rule ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difc_rule_{}_{}'.format(
+                match.group(1), match.group(2)),
+            'id': lambda match, i_group: 'diffusion_coefficient_rule_species_{}_state_{}'.format(
+                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2)),
+            'description': lambda match, i_group: 'Diffusion coefficient rule for species "{}" in state "{}"'.format(
+                match.group(1), match.group(2)),
+            'macro': lambda match: 'difc_rule {}({})'.format(
+                match.group(1), match.group(2)),
+            'arguments': lambda match: match.group(3),
+        },
+    },
+    {
+        'regex': r'^difm ([^ \(\)]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difm_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'membrane_diffusion_coefficient_species_{}'.format(match.group(1)),
+            'description': lambda match, i_group: 'Membrane diffusion coefficient of species "{}"'.format(match.group(1)),
+            'macro': lambda match: 'difm {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^difm ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difm_{}_{}'.format(match.group(1), match.group(2)),
+            'id': lambda match, i_group: 'membrane_diffusion_coefficient_species_{}_state_{}'.format(
+                match.group(1), match.group(2)),
+            'description': lambda match, i_group: 'Membrane diffusion coefficient of species "{}" in state "{}"'.format(
+                match.group(1), match.group(2)),
+            'macro': lambda match: 'difm {}({})'.format(match.group(1), match.group(2)),
+            'arguments': lambda match: match.group(3),
+        },
+    },
+    {
+        'regex': r'^difm_rule ([^ \(\)]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difm_rule_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'membrane_diffusion_coefficient_rule_species_{}'.format(
+                re.sub('[^a-zA-Z0-9_]', '_', match.group(1))),
+            'description': lambda match, i_group: 'Membrane diffusion coefficient rule for species "{}"'.format(match.group(1)),
+            'macro': lambda match: 'difm_rule {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^difm_rule ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
+        'macro': {
+            'group': lambda match: 'difm_rule_{}_{}'.format(match.group(1), match.group(2)),
+            'id': lambda match, i_group: 'membrane_diffusion_coefficient_rule_species_{}_state_{}'.format(
+                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2)),
+            'description': lambda match, i_group: 'Membrane diffusion coefficient rule for species "{}" in state "{}"'.format(
+                match.group(1), match.group(2)),
+            'macro': lambda match: 'difm_rule {}({})'.format(match.group(1), match.group(2)),
+            'arguments': lambda match: match.group(3),
+        },
+    },
+    {
+        'regex': r'^drift ([^ \(\)]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'drift_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'drift_species_{}'.format(match.group(1)),
+            'description': lambda match, i_group: 'Drift of species "{}"'.format(match.group(1)),
+            'macro': lambda match: 'drift {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^drift ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
+        'macro': {
+            'group': lambda match: 'drift_{}_{}'.format(match.group(1), match.group(2)),
+            'id': lambda match, i_group: 'drift_species_{}_state_{}'.format(
+                match.group(1), match.group(2)),
+            'description': lambda match, i_group: 'Drift of species "{}" in state "{}"'.format(
+                match.group(1), match.group(2)),
+            'macro': lambda match: 'drift {}({})'.format(match.group(1), match.group(2)),
+            'arguments': lambda match: match.group(3),
+        },
+    },
+    {
+        'regex': r'^drift_rule ([^ \(\)]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'drift_rule_{}'.format(match.group(1)),
+            'id': lambda match, i_group: 'drift_rule_species_{}'.format(re.sub('[^a-zA-Z0-9_]', '_', match.group(1))),
+            'description': lambda match, i_group: 'Drift rule for species "{}"'.format(match.group(1)),
+            'macro': lambda match: 'drift_rule {}'.format(match.group(1)),
+            'arguments': lambda match: match.group(2),
+        },
+    },
+    {
+        'regex': r'^drift_rule ([^ \(\)]+)\(([^ \(\)]+)\) (.*?)$',
+        'macro': {
+            'group': lambda match: 'drift_rule_{}_{}'.format(match.group(1), match.group(2)),
+            'id': lambda match, i_group: 'drift_rule_species_{}_state_{}'.format(
+                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2)),
+            'description': lambda match, i_group: 'Drift rule for species "{}" in state "{}"'.format(
+                match.group(1), match.group(2)),
+            'macro': lambda match: 'drift_rule {}({})'.format(match.group(1), match.group(2)),
+            'arguments': lambda match: match.group(3),
+        },
+    },
+    {
+        'regex': r'^surface_drift ([^ \(\)]+) ([^ ]+) ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'surface_drift_{}_{}_{}'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'id': lambda match, i_group: 'surface_drift_species_{}_surface_{}_shape_{}'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'description': lambda match, i_group: 'Surface drift of species "{}" on surface "{}" with panel shape "{}"'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'macro': lambda match: 'surface_drift {} {} {}'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'arguments': lambda match: match.group(4),
+        },
+    },
+    {
+        'regex': r'^surface_drift ([^ \(\)]+)\(([^ \(\)]+)\) ([^ ]+) ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'surface_drift_{}_{}_{}_{}'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'id': lambda match, i_group: 'surface_drift_species_{}_state_{}_surface_{}_shape_{}'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'description': lambda match, i_group: 'Surface drift of species "{}" in state "{}" on surface "{}" with panel shape "{}"'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'macro': lambda match: 'surface_drift {}({}) {} {}'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'arguments': lambda match: match.group(5),
+        },
+    },
+    {
+        'regex': r'^surface_drift_rule ([^ \(\)]+) ([^ ]+) ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'surface_drift_rule_{}_{}_{}'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'id': lambda match, i_group: 'surface_drift_rule_species_{}_surface_{}_panel_{}'.format(
+                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2), match.group(3)),
+            'description': lambda match, i_group: 'Surface drift rule for species "{}" on surface "{}" of panel shape "{}"'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'macro': lambda match: 'surface_drift_rule {} {} {}'.format(
+                match.group(1), match.group(2), match.group(3)),
+            'arguments': lambda match: match.group(4),
+        },
+    },
+    {
+        'regex': r'^surface_drift_rule ([^ \(\)]+)\(([^ \(\)]+)\) ([^ ]+) ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'surface_drift_rule_{}_{}_{}_{}'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'id': lambda match, i_group: 'surface_drift_rule_species_{}_state_{}_surface_{}_panel_{}'.format(
+                re.sub('[^a-zA-Z0-9_]', '_', match.group(1)), match.group(2), match.group(3), match.group(4)),
+            'description': lambda match, i_group: 'Surface drift rule for species "{}" in state "{}" on surface "{}" of panel shape "{}"'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'macro': lambda match: 'surface_drift_rule {}({}) {} {}'.format(
+                match.group(1), match.group(2), match.group(3), match.group(4)),
+            'arguments': lambda match: match.group(5),
+        },
+    },
+    {
+        'regex': r'^mol ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'mol_{}'.format(match.group(2)),
+            'id': lambda match, i_group: 'initial_count_species_{}'.format(re.sub(r'[^a-zA-Z0-9_]', '_', match.group(2))),
+            'description': lambda match, i_group: 'Initial count of species "{}"'.format(match.group(2)),
+            'macro': lambda match: 'mol {}'.format(match.group(2)),
+            'arguments': lambda match: match.group(1),
+        },
+    },
+    {
+        'regex': r'^compartment_mol ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'compartment_mol_{}'.format(match.group(2)),
+            'id': lambda match, i_group: 'initial_count_species_{}'.format(re.sub(r'[^a-zA-Z0-9_]', '_', match.group(2))),
+            'description': lambda match, i_group: 'Initial count of species "{}"'.format(match.group(2)),
+            'macro': lambda match: 'compartment_mol {}'.format(match.group(2)),
+            'arguments': lambda match: match.group(1),
+        },
+    },
+    {
+        'regex': r'^surface_mol ([^ ]+) (.*?)$',
+        'macro': {
+            'group': lambda match: 'surface_mol_{}'.format(match.group(2)),
+            'id': lambda match, i_group: 'initial_count_species_{}'.format(re.sub(r'[^a-zA-Z0-9_]', '_', match.group(2))),
+            'description': lambda match, i_group: 'Initial count of species "{}"'.format(match.group(2)),
+            'macro': lambda match: 'surface_mol {}'.format(match.group(2)),
+            'arguments': lambda match: match.group(1),
+        },
+    },
+]
```

## smoldyn/biosimulators/__main__.py

 * *Ordering differences only*

```diff
@@ -1,26 +1,26 @@
-''' BioSimulators-compliant command-line interface '''
-
-__author__ = 'Jonathan Karr'
-__email__ = 'karr@mssm.edu'
-
-__all__ = [
-    'App',
-    'main',
-]
-
-from . import __version__, get_simulator_version
-from .combine import exec_sedml_docs_in_combine_archive
-from biosimulators_utils.simulator.cli import build_cli
-
-App = build_cli('smoldyn', __version__,
-                'Smoldyn', get_simulator_version(), 'http://www.smoldyn.org',
-                exec_sedml_docs_in_combine_archive)
-
-
-def main():
-    with App() as app:
-        app.run()
-
-
-if __name__ == '__main__':
-    main()
+''' BioSimulators-compliant command-line interface '''
+
+__author__ = 'Jonathan Karr'
+__email__ = 'karr@mssm.edu'
+
+__all__ = [
+    'App',
+    'main',
+]
+
+from . import __version__, get_simulator_version
+from .combine import exec_sedml_docs_in_combine_archive
+from biosimulators_utils.simulator.cli import build_cli
+
+App = build_cli('smoldyn', __version__,
+                'Smoldyn', get_simulator_version(), 'http://www.smoldyn.org',
+                exec_sedml_docs_in_combine_archive)
+
+
+def main():
+    with App() as app:
+        app.run()
+
+
+if __name__ == '__main__':
+    main()
```

## Comparing `smoldyn-2.72.dev202307112341.dist-info/RECORD` & `smoldyn-2.72.dev202307112342.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-smoldyn/smoldyn.py,sha256=rWXvw8mk_3AGAumWOaspnMhjpQIAASaKWz5KVQ2TH0g,78575
-smoldyn/__init__.py,sha256=M-TlwaTuMxfbkRrmdKCNfgKKLgwnxqvyuto4jFkF8_0,218
-smoldyn/types.py,sha256=f5V2ONb7or4vFKLCi_gyCL6vtqdvn1j5MinFmyFxi48,1155
-smoldyn/utils.py,sha256=FEye-64lUjKWWZKs_iwa_1AfgR6EgzVGEjEJh2xy6uM,1098
-smoldyn/_smoldyn.cpython-39-darwin.so,sha256=u1YvCDkasYZBcFNrPezYLpYfvyBXBkfee0R5MeAoFDU,1923696
-smoldyn/__main__.py,sha256=8GdoclcDUTM2_2p3TI0v21F_gdyg3N5YI0OQ4F_DW_A,841
-smoldyn/biosimulators/combine.py,sha256=2m4yog8Y77C6n1w-pnikpicV5NNYSV5Rkk_t-f7zbnQ,47576
-smoldyn/biosimulators/_version.py,sha256=eT1k6c8OBrlqv4P7Qh0ph6Dj0_vBxHbKju40OzX4Vrs,46
-smoldyn/biosimulators/__init__.py,sha256=ZKoECJogmIu1M5uUEeOnOdtRmspG-Ec2VavUbcTc--w,489
-smoldyn/biosimulators/data_model.py,sha256=a3brP8Wgiusf3ngBRshnuBnCEXrKXgg-bqJN94j70jY,5274
-smoldyn/biosimulators/utils.py,sha256=vKVl1OmRbKL4_L5Ezb8rz8v0aEg7yLFpdQuOoIDPCsQ,17016
-smoldyn/biosimulators/__main__.py,sha256=4-_br6ucbpkouf2XNHpd85K2SSUz9VGkbJ-xhfxTRXI,579
-smoldyn/.dylibs/liblzma.5.dylib,sha256=ikmQg-1L7hMc2m8Amt-D1u526k9udqY4ms_H13PlP1M,201664
-smoldyn/.dylibs/libzstd.1.5.5.dylib,sha256=1rK-RHnyRX6mTsxlsO-eD4rxrC0X4DQowhhfYUjxQ2w,867440
-smoldyn/.dylibs/libtiff.6.dylib,sha256=awWpEuGNpkXdvOwPdbkaovPdwj5A8yUhUuErBrtH3JQ,538560
-smoldyn/.dylibs/libjpeg.8.2.2.dylib,sha256=TdO1bGXcSt6S22l6MwQ1PXJAJkrkoxVfKeVPvs_r5DA,689760
-smoldyn-2.72.dev202307112341.dist-info/RECORD,,
-smoldyn-2.72.dev202307112341.dist-info/WHEEL,sha256=gLMIhXBpBjiTBuxyEGSD670jZeW105GzVI8dTDaHeRg,109
-smoldyn-2.72.dev202307112341.dist-info/top_level.txt,sha256=2FmedD0M8FnH4zNLmZCw84tbGuurvZfurkH4l4zSybQ,8
-smoldyn-2.72.dev202307112341.dist-info/METADATA,sha256=jd-fefD4wVQO2aEnpuuKx5gLKjOtNFYNnlpC7nCsRHk,2856
+smoldyn/__init__.py,sha256=R3kO3jvZPyQEWwfy9LhSlz-tr0XbA6hg9gdzGXm-fTw,227
+smoldyn/__main__.py,sha256=XjjwMjJR-UjthM2oWeAlrWIe7lQqohNrf4XOxbPKtR4,868
+smoldyn/_smoldyn.cp39-win_amd64.pyd,sha256=s9kLDQr-u8ZYO5UHEb0ExTz2C_fSO4gHkk0XKAPOyaI,1925632
+smoldyn/smoldyn.py,sha256=xOQCuC8blS9ytkVksRLXAjWV3prfgcTqlE64Y6zr768,80975
+smoldyn/types.py,sha256=VsMX56PF0mLvrMbn8p8ESBbYNJS3JtxJjpsQu-MMc50,1193
+smoldyn/utils.py,sha256=kQOHH7tLa9GjGsQb3e-5OfZLI_ssUjQ4EQEkN22wrOc,1141
+smoldyn/biosimulators/__init__.py,sha256=RG9Po9HQQy69-gQ5CQbxIIKIvqSPl2Lo3wlisENXe_M,510
+smoldyn/biosimulators/__main__.py,sha256=jivj09s_B0_NQajKBYZqbuHUJaS5GqEG0kykFa5fjww,605
+smoldyn/biosimulators/_version.py,sha256=FGh8vjjI-zkppjv7VjT8sKokqXeqK0jHeQzUVjlSMhk,47
+smoldyn/biosimulators/combine.py,sha256=gtxCePSZuJeCNEfwJSg0SXTAXb8il9uLlV4vXAAXivk,48535
+smoldyn/biosimulators/data_model.py,sha256=AWnWrZBADKzCux4FWHeFzAkN7vEZUzn07ldYmzPVlPo,5443
+smoldyn/biosimulators/utils.py,sha256=xR1a7oj_ZaRhAkZhshNB1n2Jiaxv8odDTLK5CJT6vL4,17365
+smoldyn-2.72.dev202307112342.dist-info/METADATA,sha256=spaGHNIO4Z5psF7SHai60Fpnd2HGKLu-hPDG8z1pMIE,2931
+smoldyn-2.72.dev202307112342.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+smoldyn-2.72.dev202307112342.dist-info/top_level.txt,sha256=2FmedD0M8FnH4zNLmZCw84tbGuurvZfurkH4l4zSybQ,8
+smoldyn-2.72.dev202307112342.dist-info/RECORD,,
```

## Comparing `smoldyn-2.72.dev202307112341.dist-info/METADATA` & `smoldyn-2.72.dev202307112342.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-Metadata-Version: 2.1
-Name: smoldyn
-Version: 2.72.dev202307112341
-Summary: Python package for the Smoldyn simulator
-Home-page: http://www.smoldyn.org/
-Author: Dilawar Singh
-Author-email: dilawar.s.rajput@gmail.com
-License: GNU LGPLv3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: dataclasses ; python_version == "3.6"
-Provides-Extra: biosimulators
-Requires-Dist: biosimulators-utils[logging] (>=0.1.124) ; extra == 'biosimulators'
-Requires-Dist: numpy ; extra == 'biosimulators'
-Requires-Dist: pandas ; extra == 'biosimulators'
-Provides-Extra: biosimulators-dev
-Requires-Dist: flake8 ; extra == 'biosimulators-dev'
-Provides-Extra: biosimulators-tests
-Requires-Dist: python-dateutil ; extra == 'biosimulators-tests'
-Provides-Extra: dev
-Requires-Dist: mypy ; extra == 'dev'
-Requires-Dist: pyflakes ; extra == 'dev'
-Requires-Dist: black ; extra == 'dev'
-Requires-Dist: numpy ; extra == 'dev'
-Requires-Dist: matplotlib ; extra == 'dev'
-Requires-Dist: flaky ; extra == 'dev'
-
-[![Test status](https://github.com/ssandrews/Smoldyn/actions/workflows/linux.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/linux.yml)
-[![Linux build status](https://github.com/ssandrews/Smoldyn/actions/workflows/wheels_linux.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/wheels_linux.yml)
-[![OS X build status](https://github.com/ssandrews/Smoldyn/actions/workflows/osx.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/osx.yml)
-[![Windows build status](https://github.com/ssandrews/Smoldyn/actions/workflows/windows.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/windows.yml)
-[![PyPI version](https://badge.fury.io/py/smoldyn.svg)](https://badge.fury.io/py/smoldyn)
-[![BioSimulators](https://img.shields.io/badge/BioSimulators-registered-brightgreen)](https://biosimulators.org/simulators/smoldyn)
-[![runBioSimulations](https://img.shields.io/badge/runBioSimulations-simulate-brightgreen)](https://run.biosimulations.org/run)
-[![Documentation status](https://readthedocs.org/projects/smoldyn/badge/?version=latest)](https://smoldyn.readthedocs.io/en/latest/?badge=latest)
-
-# Smoldyn
-
-Smoldyn is a particle-based biochemical simulator for modeling molecular
-diffusion, surface interactions, and chemical reactions.
-
-More information about Smoldyn is available at http://www.smoldyn.org. 
-Please visit this website to learn about Smoldyn, download the latest
-release, etc.
-
+Metadata-Version: 2.1
+Name: smoldyn
+Version: 2.72.dev202307112342
+Summary: Python package for the Smoldyn simulator
+Home-page: http://www.smoldyn.org/
+Author: Dilawar Singh
+Author-email: dilawar.s.rajput@gmail.com
+License: GNU LGPLv3
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: dataclasses ; python_version == "3.6"
+Provides-Extra: biosimulators
+Requires-Dist: biosimulators-utils[logging] (>=0.1.124) ; extra == 'biosimulators'
+Requires-Dist: numpy ; extra == 'biosimulators'
+Requires-Dist: pandas ; extra == 'biosimulators'
+Provides-Extra: biosimulators-dev
+Requires-Dist: flake8 ; extra == 'biosimulators-dev'
+Provides-Extra: biosimulators-tests
+Requires-Dist: python-dateutil ; extra == 'biosimulators-tests'
+Provides-Extra: dev
+Requires-Dist: mypy ; extra == 'dev'
+Requires-Dist: pyflakes ; extra == 'dev'
+Requires-Dist: black ; extra == 'dev'
+Requires-Dist: numpy ; extra == 'dev'
+Requires-Dist: matplotlib ; extra == 'dev'
+Requires-Dist: flaky ; extra == 'dev'
+
+[![Test status](https://github.com/ssandrews/Smoldyn/actions/workflows/linux.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/linux.yml)
+[![Linux build status](https://github.com/ssandrews/Smoldyn/actions/workflows/wheels_linux.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/wheels_linux.yml)
+[![OS X build status](https://github.com/ssandrews/Smoldyn/actions/workflows/osx.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/osx.yml)
+[![Windows build status](https://github.com/ssandrews/Smoldyn/actions/workflows/windows.yml/badge.svg)](https://github.com/ssandrews/Smoldyn/actions/workflows/windows.yml)
+[![PyPI version](https://badge.fury.io/py/smoldyn.svg)](https://badge.fury.io/py/smoldyn)
+[![BioSimulators](https://img.shields.io/badge/BioSimulators-registered-brightgreen)](https://biosimulators.org/simulators/smoldyn)
+[![runBioSimulations](https://img.shields.io/badge/runBioSimulations-simulate-brightgreen)](https://run.biosimulations.org/run)
+[![Documentation status](https://readthedocs.org/projects/smoldyn/badge/?version=latest)](https://smoldyn.readthedocs.io/en/latest/?badge=latest)
+
+# Smoldyn
+
+Smoldyn is a particle-based biochemical simulator for modeling molecular
+diffusion, surface interactions, and chemical reactions.
+
+More information about Smoldyn is available at http://www.smoldyn.org. 
+Please visit this website to learn about Smoldyn, download the latest
+release, etc.
+
+
+
```

