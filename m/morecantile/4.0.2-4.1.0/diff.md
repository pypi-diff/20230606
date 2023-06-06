# Comparing `tmp/morecantile-4.0.2.tar.gz` & `tmp/morecantile-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-4.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "morecantile-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-4.0.2.tar` & `morecantile-4.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      215 2023-05-31 16:47:47.711505 morecantile-4.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-05-31 16:47:47.711505 morecantile-4.0.2/.gitignore
--rw-r--r--   0        0        0      822 2023-05-31 16:47:47.711505 morecantile-4.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-31 16:47:47.711505 morecantile-4.0.2/LICENSE
--rw-r--r--   0        0        0     5305 2023-05-31 16:47:47.711505 morecantile-4.0.2/README.md
--rw-r--r--   0        0        0      436 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/commons.py
--rw-r--r--   0        0        0     7267 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/CanadianNAD83_LCC.json
--rw-r--r--   0        0        0     4679 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5176 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     8457 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/README.md
--rw-r--r--   0        0        0     7374 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     7365 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     7367 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6932 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/WGS1984Quad.json
--rw-r--r--   0        0        0     7843 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     7072 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/WorldCRS84Quad.json
--rw-r--r--   0        0        0     7001 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1748 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/defaults.py
--rw-r--r--   0        0        0      907 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/errors.py
--rw-r--r--   0        0        0    40237 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16657 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3364 2023-05-31 16:47:47.715505 morecantile-4.0.2/morecantile/utils.py
--rw-r--r--   0        0        0     2295 2023-05-31 16:47:47.715505 morecantile-4.0.2/pyproject.toml
--rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0      215 2023-06-06 16:11:11.947318 morecantile-4.1.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-06-06 16:11:11.947318 morecantile-4.1.0/.gitignore
+-rw-r--r--   0        0        0      822 2023-06-06 16:11:11.947318 morecantile-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-06-06 16:11:11.947318 morecantile-4.1.0/LICENSE
+-rw-r--r--   0        0        0     5305 2023-06-06 16:11:11.947318 morecantile-4.1.0/README.md
+-rw-r--r--   0        0        0      436 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/commons.py
+-rw-r--r--   0        0        0     7267 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0     5176 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-06-06 16:11:11.947318 morecantile-4.1.0/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1748 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/errors.py
+-rw-r--r--   0        0        0    41068 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-06-06 16:11:11.951318 morecantile-4.1.0/morecantile/utils.py
+-rw-r--r--   0        0        0     2295 2023-06-06 16:11:11.951318 morecantile-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.1.0/PKG-INFO
```

### Comparing `morecantile-4.0.2/.gitignore` & `morecantile-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/.pre-commit-config.yaml` & `morecantile-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/LICENSE` & `morecantile-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/README.md` & `morecantile-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/commons.py` & `morecantile-4.1.0/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-4.1.0/morecantile/data/CanadianNAD83_LCC.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/EuropeanETRS89_LAEAQuad.json` & `morecantile-4.1.0/morecantile/data/EuropeanETRS89_LAEAQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-4.1.0/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/NZTM2000Quad.json` & `morecantile-4.1.0/morecantile/data/NZTM2000Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/UPSAntarcticWGS84Quad.json` & `morecantile-4.1.0/morecantile/data/UPSAntarcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/UPSArcticWGS84Quad.json` & `morecantile-4.1.0/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/UTM31WGS84Quad.json` & `morecantile-4.1.0/morecantile/data/UTM31WGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/WGS1984Quad.json` & `morecantile-4.1.0/morecantile/data/WGS1984Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/WebMercatorQuad.json` & `morecantile-4.1.0/morecantile/data/WebMercatorQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/WorldCRS84Quad.json` & `morecantile-4.1.0/morecantile/data/WorldCRS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/data/WorldMercatorWGS84Quad.json` & `morecantile-4.1.0/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/defaults.py` & `morecantile-4.1.0/morecantile/defaults.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/errors.py` & `morecantile-4.1.0/morecantile/errors.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/models.py` & `morecantile-4.1.0/morecantile/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,26 @@
     Sequence,
     Tuple,
     Union,
 )
 
 from cachetools import LRUCache, cached
 from cachetools.keys import hashkey
-from pydantic import AnyHttpUrl, BaseModel, Field, PrivateAttr, conlist, validator
+from pydantic import (
+    AnyHttpUrl,
+    AnyUrl,
+    BaseModel,
+    Field,
+    PrivateAttr,
+    conlist,
+    root_validator,
+    validator,
+)
 from pyproj import CRS, Transformer
-from pyproj.exceptions import ProjError
+from pyproj.exceptions import CRSError, ProjError
 
 from morecantile.commons import BoundingBox, Coords, Tile
 from morecantile.errors import (
     DeprecationError,
     InvalidZoomError,
     NoQuadkeySupport,
     PointOutsideTMSBounds,
@@ -46,52 +55,64 @@
 
 if TYPE_CHECKING:
     axesInfo = List[str]
 else:
     axesInfo = conlist(str, min_items=2, max_items=2)
 
 
-class CRSType(CRS, str):
-    """
-    A geographic or projected coordinate reference system.
-    """
+class CRSUri(BaseModel):
+    """Coordinate Reference System (CRS) from URI."""
 
-    @classmethod
-    def __get_validators__(cls):
-        """validator for the type."""
-        yield cls.validate
+    uri: AnyUrl = Field(
+        ...,
+        description="Reference to one coordinate reference system (CRS) as URI",
+        examples=[
+            "http://www.opengis.net/def/crs/EPSG/0/3978",
+            "urn:ogc:def:crs:EPSG::2193",
+        ],
+    )
 
-    @classmethod
-    def validate(cls, value: Union[CRS, str]) -> CRS:
-        """Validate CRS."""
-        # If input is a string we translate it to CRS
-        # TODO: add NotImplementedError for ISO 19115
-        if not isinstance(value, CRS):
-            return CRS.from_user_input(value)
 
-        return value
+class CRSWKT(BaseModel):
+    """Coordinate Reference System (CRS) from WKT."""
 
-    @classmethod
-    def __modify_schema__(cls, field_schema):
-        """Update default schema."""
-        field_schema.update(
-            anyOf=[
-                {"type": "pyproj.CRS"},
-                {"type": "string", "minLength": 1, "maxLength": 65536},
-            ],
-            examples=[
-                "CRS.from_epsg(4326)",
-                "http://www.opengis.net/def/crs/EPSG/0/3978",
-                "urn:ogc:def:crs:EPSG::2193",
-            ],
-        )
+    wkt: str = Field(
+        ...,
+        description="Reference to one coordinate reference system (CRS) as WKT string",
+        examples=[
+            'GEOGCS["GCS_WGS_1984",DATUM["D_WGS_1984",SPHEROID["WGS_1984",6378137,298.257223563]],PRIMEM["Greenwich",0],UNIT["Degree",0.017453292519943295]]',
+        ],
+    )
 
-    def __repr__(self):
-        """Type representation."""
-        return f"CRS({super().__repr__()})"
+
+# NOT SUPPORTED
+# class CRSRef(BaseModel):
+#     """CRS from referenceSystem."""
+#
+#     referenceSystem: Dict[str, Any] = Field(
+#         ...,
+#         description="A reference system data structure as defined in the MD_ReferenceSystem of the ISO 19115",
+#     )
+
+
+class CRSType(BaseModel):
+    """CRS model.
+
+    Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/common-geodata/crs.yaml
+
+    Code generated using https://github.com/koxudaxi/datamodel-code-generator/
+    """
+
+    __root__: Union[str, Union[CRSUri, CRSWKT]] = Field(..., title="CRS")
+
+    @root_validator
+    def validate_crs(cls, values):
+        """Make sure the CRS can be used in Pyproj."""
+        assert CRS.from_user_input(values.get("__root__"))
+        return values
 
 
 def CRS_to_uri(crs: CRS) -> str:
     """Convert CRS to URI."""
     authority = "EPSG"
     code = None
     version = "0"
@@ -131,15 +152,14 @@
     crs: Optional[CRSType]
     orderedAxes: Optional[axesInfo]
 
     class Config:
         """Configure TMSBoundingBox."""
 
         arbitrary_types_allowed = True
-        json_encoders = {CRS: lambda v: CRS_to_uri(v)}
 
 
 # class variableMatrixWidth(BaseModel):
 #     """Variable Matrix Width Definition
 
 
 #     ref: https://github.com/opengeospatial/2D-Tile-Matrix-Set/blob/master/schemas/tms/2.0/json/variableMatrixWidth.json
@@ -252,43 +272,43 @@
     )
     tileMatrices: List[TileMatrix] = Field(
         ..., description="Describes scale levels and its tile matrices"
     )
 
     # Private attributes
     _is_quadtree: bool = PrivateAttr()
-    _geographic_crs: CRSType = PrivateAttr(default=WGS84_CRS)
+    _crs: CRS = PrivateAttr()
+    _geographic_crs: CRS = PrivateAttr(default=WGS84_CRS)
     _to_geographic: Transformer = PrivateAttr()
     _from_geographic: Transformer = PrivateAttr()
 
     class Config:
         """Configure TileMatrixSet."""
 
         arbitrary_types_allowed = True
-        json_encoders = {CRS: lambda v: CRS_to_uri(v)}
 
     def __init__(self, **data):
         """Create PyProj transforms and check if TileMatrixSet supports quadkeys."""
         if {"supportedCRS", "topLeftCorner"}.intersection(data):
             raise DeprecationError(
                 "Tile Matrix Set must be version 2.0. Use morecantile <4.0 for TMS 1.0 support"
             )
 
         super().__init__(**data)
 
         self._is_quadtree = check_quadkey_support(self.tileMatrices)
-
+        self._crs = CRS.from_user_input(self.crs.__root__)
         self._geographic_crs = data.get("_geographic_crs", WGS84_CRS)
 
         try:
             self._to_geographic = Transformer.from_crs(
-                self.crs, self._geographic_crs, always_xy=True
+                self._crs, self._geographic_crs, always_xy=True
             )
             self._from_geographic = Transformer.from_crs(
-                self._geographic_crs, self.crs, always_xy=True
+                self._geographic_crs, self._crs, always_xy=True
             )
         except ProjError:
             warnings.warn(
                 "Could not create coordinate Transformer from input CRS to the given geographic CRS"
                 "some methods might not be available.",
                 UserWarning,
             )
@@ -303,25 +323,25 @@
     def __iter__(self):
         """Iterate over matrices"""
         for matrix in self.tileMatrices:
             yield matrix
 
     def __repr__(self):
         """Simplify default pydantic model repr."""
-        return f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self.crs}>"
+        return f"<TileMatrixSet title='{self.title}' id='{self.id}' crs='{self._crs}>"
 
     @property
     def geographic_crs(self) -> CRSType:
         """Return the TMS's geographic CRS."""
         return self._geographic_crs
 
     @property
     def rasterio_crs(self):
         """Return rasterio CRS."""
-        return to_rasterio_crs(self.crs)
+        return to_rasterio_crs(self._crs)
 
     @property
     def rasterio_geographic_crs(self):
         """Return the geographic CRS as a rasterio CRS."""
         return to_rasterio_crs(self._geographic_crs)
 
     @property
@@ -336,15 +356,15 @@
 
     @property
     def _invert_axis(self) -> bool:
         """Check if CRS has inverted AXIS (lat,lon) instead of (lon,lat)."""
         return (
             ordered_axis_inverted(self.orderedAxes)
             if self.orderedAxes
-            else crs_axis_inverted(self.crs)
+            else crs_axis_inverted(self._crs)
         )
 
     @classmethod
     def from_v1(cls, tms: Dict) -> "TileMatrixSet":
         """
         Makes a TMS from a v1 TMS definition
 
@@ -489,16 +509,29 @@
                         "tileHeight": tile_height,
                         "matrixWidth": matrix_scale[0] * 2**zoom,
                         "matrixHeight": matrix_scale[1] * 2**zoom,
                     }
                 )
             )
 
+        if crs.to_authority(min_confidence=20):
+            crs_str = CRS_to_uri(crs)
+
+            # Some old Proj version might not support URI
+            # so we fall back to wkt
+            try:
+                CRS.from_user_input(crs_str)
+            except CRSError:
+                crs_str = crs.to_wkt()
+
+        else:
+            crs_str = crs.to_wkt()
+
         return cls(
-            crs=crs,
+            crs=crs_str,
             tileMatrices=tile_matrices,
             id=id,
             title=title,
             _geographic_crs=geographic_crs,
             **kwargs,
         )
 
@@ -551,15 +584,15 @@
         Tile resolution for a TileMatrix.
 
         From note g in http://docs.opengeospatial.org/is/17-083r2/17-083r2.html#table_2:
           The pixel size of the tile can be obtained from the scaleDenominator
           by multiplying the later by 0.28 10-3 / metersPerUnit.
 
         """
-        return matrix.scaleDenominator * 0.28e-3 / meters_per_unit(self.crs)
+        return matrix.scaleDenominator * 0.28e-3 / meters_per_unit(self._crs)
 
     def zoom_for_res(
         self,
         res: float,
         max_z: Optional[int] = None,
         zoom_level_strategy: str = "auto",
         min_z: Optional[int] = None,
@@ -832,15 +865,15 @@
 
         return BoundingBox(left, bottom, right, top)
 
     @property
     @cached(  # type: ignore
         LRUCache(maxsize=512),
         key=lambda self: hashkey(
-            self.crs,
+            self.crs.__root__,
             self.tileMatrices[0].pointOfOrigin,
             self.tileMatrices[0].matrixWidth,
             self.tileMatrices[0].matrixHeight,
         ),
     )
     def bbox(self):
         """Return TMS bounding box in geographic coordinate reference system."""
@@ -998,26 +1031,26 @@
             "type": "Feature",
             "bbox": bbox,
             "id": xyz,
             "geometry": geom,
             "properties": {
                 "title": f"XYZ tile {xyz}",
                 "grid_name": self.id,
-                "grid_crs": self.crs.to_string(),
+                "grid_crs": self.crs.__root__,
             },
         }
 
         if projected:
             warnings.warn(
                 "CRS is no longer part of the GeoJSON specification."
                 "Other projection than EPSG:4326 might not be supported.",
                 UserWarning,
             )
             feat.update(
-                {"crs": {"type": "EPSG", "properties": {"code": self.crs.to_epsg()}}}
+                {"crs": {"type": "EPSG", "properties": {"code": self._crs.to_epsg()}}}
             )
 
         if props:
             feat["properties"].update(props)
 
         if fid is not None:
             feat["id"] = fid
```

### Comparing `morecantile-4.0.2/morecantile/scripts/cli.py` & `morecantile-4.1.0/morecantile/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/morecantile/utils.py` & `morecantile-4.1.0/morecantile/utils.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/pyproject.toml` & `morecantile-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morecantile-4.0.2/PKG-INFO` & `morecantile-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 4.0.2
+Version: 4.1.0
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: morecantile Version: 4.0.2 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 4.1.0 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

