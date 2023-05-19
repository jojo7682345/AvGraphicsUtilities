# AvGraphicsUtilities
A GUI library in written in C using Vulkan and GLFW

## Goals for the project
 - Use the GUI library to make a Visual Editor for UI design
 - Making a simple IDE
 - Migrate project from Visual Studio
 - Linux and rpi support
 - Add embedded system support (replace vulkan renderer with cpu renderer based on platform)

## Tasks
- [ ] Renderer
    - [ ] Render rectangles
        - [ ] Basic Transform buffer input
        - [ ] Basic Mesh input
        - [ ] Basic Shaders
        - [ ] Color input
    - [ ] Render images
        - [ ] Image loading
        - [ ] Storing images on gpu
    - [ ] Render text
        - [ ] font loading
        - [ ] font rendering
- [ ] Positioner
    - [ ] Create Layouts 
        - [ ] Make absolute positioner
        - [ ] Make grid positioner
        - [ ] Make split positioner
        - [ ] *Make floating positioner*
    - [ ] Create Positioning Chain
- [ ] Component handler
    - [ ] Component creation
    - [ ] Component destruction
    - [ ] Component pooling
- [ ] .ui parser
    - [x] tokenizer
    - [ ] lexer
    - [ ] preprocessor
    - [ ] scemantic analysis
    - [ ] operation order generation

## Building
clone the repository and run the following commands
```bash
gcc build/builder.c -o builder
./builder build
sudo ./builder install
```
the test executable should appear in AvGraphicsUtilities
