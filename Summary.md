# Summary
### 1. Mini Game subpackages restrictions :
The total size of all subpackages of a Mini Game cannot exceed 16 MB. A single subpackage or main package cannot exceed 4 MB.

### 2. Local user file restrictions :
Mini Programs can store up to 50 MB.

### 3. JavaScript restrictions :
JS code cannot be executed via eval. No functions can be created with 'new Function'.

### 4. Rendering restrictions:
You can use the Canvas.getContext('2d') API to get the CanvasRenderingContext2D object. Most of the properties and methods defined by HTML Canvas 2D Context are implemented. You can use the Canvas.getContext('webgl') API to get the WebGLRenderingContext object. All the properties, methods, and constants defined by WebGL 1.0 are implemented.

### 5. Compressed Textures:
iOS supports the PVR format and Android supports the ETC1 format.

### 6. BOM or DOM restrictions:
Environments do NOT support BOM or DOM, they do not have global document and window objects. Therefore, if you want to use DOM APIs to create a canvas, image, or other elements, an error will be reported. The Mini Game runtime environment is a host environment different from a browser. It does not provide BOM and DOM APIs, but does provide wx APIs. Using wx APIs, developers can call native capabilities, such as drawing, audio/video, network, and documents.
