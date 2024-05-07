# Kaleidoscope Mesh
This asset draws a variety of beautiful kaleidoscope meshes. Highly customizable and fast processing.

# Getting started
- Create empty GameObject and attach KaleidoscopeMeshRenderer component to it.
- Change "Target Position". Then the kaleidoscope will move.
- Modify or add elements to the Shape list. Then, the kaleidoscope pattern will change. Elements in the Shape list are executed from top to bottom.
  - Chain shape : Duplicate parts at equal intervals. Adding an angle creates a curve.
  - Circle shape : Duplicate parts in a circle.
  - Mirror shape : Duplicate parts by mirroring it.

# Note
- To use all features, please turn on "Read/Write" for the mesh.
- Turning on "Enable GPU Instancing" for the material will optimize the drawing process.
- "Instance Limit" prevents Editor from freezing due to number explosion. Increase this value if you want to display more parts.
- Compatible with animation.
- When using a material for particles, you can change the color by turning on "Override Vertex Color".

# Advanced
You can create a Shape class. Please inherit Shape and implement the function. You need to add a reference to KaleidoscopeMesh in your AssemblyDefinition. The classes created will be automatically recognized.
