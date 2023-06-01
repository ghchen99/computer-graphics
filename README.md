# Computer Graphics Coding
This project focuses on various computer graphics coding tasks, including illumination and shading, texture mapping, bump mapping, render-to-texture, and GPU ray tracing. Each task involves implementing different techniques to enhance the visual quality and realism of rendered scenes.

This project was completed using the Web version of the Open Graphics Library (WebGL) and the OpenGL Shading Language (GLSL).

## Task 3: Illumination and Shading
## Task 3a: Per Vertex Gouraud shading
In this task, Gouraud shading is implemented using per-polygon vertex and fragment shaders. The shaders perform operations on scene vertices in object space. The vertex shader defines interfaces to pass specific information about the currently processed vertex to the fragment shader. The lighting properties, such as ambient, diffuse, specular, and shininess, are defined using uniform variables.

## Task 3b: Per Pixel Phong shading
Phong shading is implemented in this task, which interpolates normal vectors for each fragment instead of interpolated colors. The shading effect depends on the viewer's position, fragment's position, and light position. Similar to Task 3a, the necessary interfaces and lighting properties are defined using uniform variables.

## Task 3c: Per Pixel Toon shading
Toon shading, a simple lighting scheme to achieve cartoon-like effects, is implemented in this task. Similar to Task 3b, it operates directly on fragments and requires extensions in the per-polygon fragment shader. Preprocessor definitions are used to switch between different shading types.

## Task 3d: Blinn-Phong (not assessed)
Blinn-Phong shading, a more efficient modification of Phong shading using halfway-vectors, is implemented in this task. It aims to approximate illumination more efficiently.

## Task 5: Texture
## Task 5a: Texture
This task focuses on applying textures to objects. UV texture coordinates are used to map the texture onto the object. A 2D texture sampler object is defined as a uniform variable in the per-polygon fragment shader to handle the texture. The result is a textured object with ambient lighting.

## Task 5b: Bump mapping
Bump mapping is implemented in this task to create the illusion of highly tessellated surfaces. Instead of RGB color values, a separate texture encodes surface normals. These normals are used in the Phong illumination model to achieve realistic lighting effects.

## Task 5c: Render to Texture
This task introduces the concept of render-to-texture (R2T) fragment shaders. The scene is rendered into a framebuffer, allowing for post-processing operations on the 2D texture image. A simple blur effect is implemented by sampling the texture towards the image center.

## Task 6: GPU Ray Tracing
## Task 6a: Simple GPU ray tracing
In this task, a simple ray tracer is implemented using the R2T fragment shader. The scene consists of planes and spheres defined mathematically. The R2T vertex shader is adjusted to produce a fixed aspect ratio, and rays are virtually shot into the scene. The resulting image simulates ray-traced rendering of the objects.

## Getting Started
To run the computer graphics coding tasks, follow these steps:

- Clone the repository: git clone https://github.com/your-username/computer-graphics-coding.git
- Set up a local web server or use an online development environment.
- Open the project in your preferred web development environment.
- Navigate to the respective task files and shaders to modify and experiment with different techniques.
- Run the project on your web server to visualize the results.
- Make sure to check the specific task instructions within the code comments for any additional setup or configuration requirements.

## Contributors
If you would like to contribute to the project, feel free to open a pull request or submit an issue.

## License
This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the license terms.
