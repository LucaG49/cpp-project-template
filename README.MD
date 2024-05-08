# Project Template (C++)

This is a basic template that i use for C++ projects with CMake and Vcpkg. It can be used as a starting point for new C++ projects.

## Prerequisites

- **CMake**: Make sure you have CMake installed on your system. You can download it from [here](https://cmake.org/download/).
- **Vcpkg**: Ensure you have Vcpkg installed and configured on your system. You can find instructions on how to install Vcpkg [here](https://github.com/microsoft/vcpkg). Please install in path "C:/vcpkg/"
- **Visual Studio Code**: Make sure you have installed the CMake and C++ extension.
- **Visual Studio 17 2022 generator**: CMake is configured with Visual Studio 17 2022.

## Project Structure
```
cpp-project-template/
│
├───.vscode/                // Configuration files for Visual Studio Code
│   ├───settings.json       // Project settings
│   └───task.json           // Task configuration
│
├───build/                  // Output directory for object files and executables
│
├───docs/                   // Notes, instructions, and documentation
│   ├───design_document.pdf
│   ├───instructions.md
│   └───notes.txt
│
├───include/                // Header files (.h)
│   ├───core/               // Header files for core
│   ├───gui/                // Header files for GUI
│   ├───network/            // Header files for network management
│   └───utils/              // Header files for utility functions
│
├───lib/                    // External libraries (if needed)
│   ├───library1/
│   └───library2/
│
├───resources/              // Images, icons, and other non-code files
│   ├───icons/
│   │   ├───icon1.png
│   │   └───icon2.png
│   └───images/
│       ├───background.jpg
│       └───logo.png
│
├───src/                    // C++ source code
│    ├───core/               // Source code for core logic
│    │   ├───core_functions.cpp  // Other core source files
│    │   └───main.cpp        // Main source file
│    │
│    ├───gui/                // Source code for graphical user interface
│    │   ├───main_window.cpp
│    │   └───widgets/        // GUI components
│    │       ├───button.cpp
│    │       └───textbox.cpp
│    │
│    ├───network/            // Source code for network management
│    │   ├───network_manager.cpp
│    │   └───protocol/       // Network protocol implementations
│    │       ├───http.cpp
│    │       └───tcp.cpp
│    │
│    └───utils/              // Source code for utility functions
│        └───utility_functions.cpp
│  
├── .gitignore
├── CMakeLists.txt
├── CMakePresets.json
├── LICENSE
├── README.MD
├── vcpkg-configuration.json
└── vcpkg.json
```

This directory structure represents the layout of the project template. Each folder and file is organized hierarchically within the `project_template` directory.

## Configuration

For detailed instructions on configuring and building the project using CMake, including GUI steps, visit the official CMake tutorial [here](https://cmake.org/runningcmake/).

To learn how to add libraries using Vcpkg, follow the steps provided in the official Vcpkg documentation [here](https://learn.microsoft.com/it-it/vcpkg/get_started/get-started?pivots=shell-cmd).

## Visual Studio Code:

1. **Ctrl+Shift+P -> CMake: Configuration**

2. **CMake: Build**

## Customization

You can customize this template to fit your specific needs. Add new source files, dependencies, or configurations as necessary.
