# The usd library 

The usd library graphs are built up with a few layers that each 
hold some core node for building usd assets and files. 

These single nodes when combined(parented or strung together)
 can build more complicated usd concepts. Please see the examples in this git repo
 for reference.

# Core layers

![Alt text](images/CoreUsdNodes.png?raw=true "CoreLayers")

### pxr_usd

##### nodes

 - CreateNew: Creates a new empty layer with the given identifier.
 - StageOpen: Attempt to find a matching existing stage in a cache if UsdStageCacheContext objects exist on the stack. Failing that, create a new stage and recursively compose prims defined within and referenced by the layer at filePath, which must already exist.
 - RootLayerSave: Save out the Root layer to a stage.
 - GetPrimAtPath: Returns the prim at the given path.
 - GetPropertyNames: Return all of this prim's property names (attributes and relationships), including all builtin properties
 - GetAttribute: Return a UsdAttribute with the name given.
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
 - BasisCurves: Construct a UsdGeom BasisCurves on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_basis_curves.html#details)
 - Cylinder: Construct a UsdGeom Cylinder on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_cylinder.html#details)
 - NurbsCurves: Construct a UsdGeom NurbsCurves on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_nurbs_curves.html#details)
 - Capsule: Construct a UsdGeom Capsule on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_capsule.html#details)
 - DefinePrim: Construct a UsdGeom DefinePrim on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_stage.html#a6151ae804f7145e451d9aafdde347730)
 - Xform: Construct a UsdGeom Xform on UsdPrim. [details](https://graphics.pixar.com/usd/docs/api/class_usd_geom_xform.html#details)

### pxr_usd_variants

##### nodes

 - AddVariantSet: Add a variant set to a prim of your choice.
 - AddVariant: Add a variant to a variant set.
 - SetVariantSelection: Set a variant selection of your choice.
 - GetVariantEditContext: Edit context to a selected variant.

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

![Alt text](images/helloworld.png?raw=true "HelloWorld")

 - [HelloWorldRedux.nxt](examples/HelloWorldRedux.nxt)
    - Please see [helloWorldRedux](https://graphics.pixar.com/usd/docs/Hello-World-Redux---Using-Generic-Prims.html) from pixar.

![Alt text](images/helloworldRedux.png?raw=true "HelloWorldRedux")

 - [AuthorVariants.nxt](examples/AuthorVariants.nxt)
    - Please see [AuthorVariants](https://graphics.pixar.com/usd/docs/Authoring-Variants.html) from pixar.

![Alt text](images/authorvariants.png?raw=true "HelloWorldRedux")