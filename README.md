# Project README

## Overview
This project is a C program designed to create a graphical user interface (GUI) for controlling a robotic arm using a mouse. The GUI is built using a custom windowing library that supports Linux, Windows, Wine, and WebAssembly.

## Features
- **Mouse Control**: Users can control the movement of the robotic arm by dragging a slider with the mouse.
- **Cross-Platform Compatibility**: The project supports building on multiple operating systems including Linux, Windows, and WebAssembly.
- **Development Tools**: Requires C/C++ compiler (GCC, Clang), Make utility, standard development tools, and specific libraries like X11 for Linux.

## Project Structure
The following files and directories exist in the project:

### Prerequisites
- **C/C++ Compiler and Debugger**: GCC or Clang.
- **Make Utility**: For building the project.
- **Standard Development Tools**.
- **Libraries**:
  - X11: For Linux GUI functionality.
  - libpng, libjpeg: For image processing in some of the build configurations.

## Build & Run
### Linux
To build and run on Linux:

```bash
cd <Project>
make -f Makefile.linux all
make -f Makefile.linux exe
```

### Windows
To build and run on Windows (using MinGW-w64):

```bash
cd <Project>
make -f Makefile.windows all
make -f Makefile.windows exe
```

### Wine
To cross-compile for Windows using Wine:

```bash
cd <Project>
make -f Makefile.wine all
make -f Makefile.wine exe
```

### WebAssembly (Emscripten)
To build and run on the web using Emscripten:

```bash
cd <Project>
make -f Makefile.web all
make -f Makefile.web exe
```

Each `Makefile.(os)` can be used to perform specific actions like cleaning, building, or executing the project.