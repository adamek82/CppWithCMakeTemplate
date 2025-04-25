# CppWithCMakeTemplate

A minimal C++ project template with CMake configuration, optimized for development in VSCode.

## Features

- CMake build system with C++20 standard.
- Preconfigured VSCode settings:
  - Build tasks (`tasks.json`).
  - Launch configuration (`launch.json`) for debugging.
  - CMake auto-configure on open (`settings.json`).
- Organized project structure:
  - `include/` for header files.
  - `src/` for source files.
  - `bin/` for build outputs.
- `.gitignore` for typical CMake and build artifacts.

## Getting Started

### Prerequisites

- [CMake](https://cmake.org/) 3.15 or newer
- [Visual Studio Code](https://code.visualstudio.com/)
  - Recommended extensions: [CMake Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools), [C++ (MSVC)](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools)

### Building the Project

1. Open the workspace (`CppWithCMakeTemplate.code-workspace`) in VSCode.
2. Allow CMake Tools to configure the project automatically.
3. Use **Ctrl+Shift+B** or select **Terminal → Run Build Task** to build the project.
4. Launch the application using the configured debugger.

Alternatively, you can build manually:

```bash
cmake -S . -B build
cmake --build build
```

The output binary will appear under `bin/`.

### Project Structure

```
CppWithCMakeTemplate/
├── .gitignore
├── .vscode/
│   ├── launch.json
│   ├── settings.json
│   └── tasks.json
├── include/
│   └── CppWithCMakeTemplate.h
├── src/
│   └── CppWithCMakeTemplate.cpp
├── CMakeLists.txt
└── CppWithCMakeTemplate.code-workspace
```

## License

This template is provided without any warranty. Feel free to use and modify it for your projects.
