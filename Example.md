# How to guide for the usd library 

The usd library graphs are built up with a few layers that each 
hold some core node for building up usd assets. 

These single nodes when combined(parented or strung together)
 can build more complicated usd concepts. Please see the examples in this git repo
 for reference.

# Core layers

### pxr_usd

##### nodes

 - CreateNew: 
 - StageOpen: 
 - RootLayerSave: 
 - GetPrimAtPath: 
 - GetPropertyNames: 
 - GetAttribute: 
 - SetAttribute: 
 - SetDefaultPrim: 
 - GetDefaultPrim: 

### pxr_usd_geom

##### nodes

 - Sphere: Construct a UsdGeom Sphere on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_sphere.html#details)
 - Cube: Construct a UsdGeom Cube on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_cube.html#details)
 - Mesh: Construct a UsdGeomMesh on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_mesh.html#details)
 - Cone: Construct a UsdGeom Cone on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_cone.html#details)
 - Points: Construct a UsdGeom Points on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_points.html#details)
 - NurbsPatch: Construct a UsdGeom NurbsPatch on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_nurbs_patch.html#details)
 - BasisCurves:
 - Cylinder:
 - NurbsCurves:
 - Capsule:
 - DefinePrim


### pxr_usd_variants

##### nodes

 - AddVariantSet: Add a variant set to a prim of your choice.
 - AddVariant: Add a variant to a variant set.
 - SetVariantSelection: Set a variant selection of your choice.
 - GetVariantEditContext: Add context to a selected variant.

### pxr_usd_model_api

##### nodes

 - SetKind: Set a kind for a usd prim
 - SetAssetName: Give a prim a asset name
 - SetAssetVersion: Give a prim an asset version

### pxr_usd_tools

##### nodes

 - UsdView: Open up a usdview form inside nxt
 - UsdCat: Open up a terminal and cat usd file from within nxt
 - UsdDiff: Open up a terminal and diff usd file from within nxt
 - UsdConvert: Convert abc/usd file to usd file type of your choice.

# Example Layers
 - The following nxt graphs build example usd file based off of Pixar's [Tutorials](https://graphics.pixar.com/usd/docs/USD-Tutorials.html).
 - [HelloWorld.nxt](examples/HelloWorld.nxt)
    - Please see [HelloWorld](https://graphics.pixar.com/usd/docs/Hello-World---Creating-Your-First-USD-Stage.html) from pixar.

 - [HelloWorldRedux.nxt](examples/HelloWorldRedux.nxt)
    - Please see [helloWorldRedux](https://graphics.pixar.com/usd/docs/Hello-World-Redux---Using-Generic-Prims.html) from pixar.

