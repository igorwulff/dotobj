<h1 align="center">dotobj 4.0.0</h1>

### @jujuadams

Lightweight .obj 3D model loader written in native GML. Can load from external files or from buffers. This example does not show off complex renderering or PBR, it only demonstrates the loading capabilities of the library.

Details on the .obj format can be found here: http://paulbourke.net/dataformats/obj/

&nbsp;

**dotobj currently supports:**

1. Per vertex position, texture coordinates, and normals

2. Materials and material libraries

3. Groups - *(objects can be parsed as groups if required)*

4. Vertex colours - *(not in the official .obj spec, but some editors can export them)*

5. UV flipping - *(for compatibility between DirectX and OpenGL)*

6. N-gon faces

7. Custom vertex buffer formats

8. Winding-order reversal

&nbsp;

**How do I import dotobj into my game?**

GameMaker Studio 2.2.3 allows you to import assets, including scripts and shaders, directly into your project via the "Local Package" system. From the [Releases](https://github.com/JujuAdams/dotobj/releases/) tab for this repo, download the .yymp file for the latest version. In the GMS2 IDE, load up your project and click on "Tools" on the main window toolbar. Select "Import Local Package" from the drop-down menu then import all scripts from the package.

&nbsp;

**Please note that dotobj doesn't support the following features:**

1. Smoothing groups

*Not a priority since you can usually bake normals on export, but it'd be useful to have regardless.*

2. Separate in-file LOD

*Not sure how often this gets used. Probably possible to implement if requested.*

3. Line primitives

*Line primitives are mostly used for visualisation in editors rather than for actual game rendering. It's possible to parse line primitives and output that, but it's not a priority.*

4. Freeform curve/surface geometry (NURBs/Bezier curves etc.)

*Rare to see this in gamedev and getting GameMaker to generates surfaces is not going to be a pleasant process. This will probably never be implemented.*
