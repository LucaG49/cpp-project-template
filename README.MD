# Project Template (C++)

This is a basic template that i use for C++ projects with CMake and Vcpkg for Windows. It can be used as a starting point for new C++ projects.

## Prerequisites

- **CMake**: Make sure you have CMake installed on your system. You can download it from [here](https://cmake.org/download/).
- **Vcpkg**: Ensure you have Vcpkg installed and configured on your system. You can find instructions on how to install Vcpkg [here](https://github.com/microsoft/vcpkg). Please install in path "C:/vcpkg/".
- **Visual Studio Code**: Make sure you have installed Visual Studio Code with extensions and compilers for C++. You can find detailed instructions here [here](https://code.visualstudio.com/docs/languages/cpp).
- **Visual Studio 17 2022 generator**: CMake is configured with Visual Studio 17 2022 generator. If you prefer to use another generator see "CMakePresets.json".

## Project Structure
```
cpp-project-template/
│
├───builds/                  // Output directory for object files and executables
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
├───tests/
│  
├── .gitignore
├── CMakeLists.txt
├── CMakePresets.json
├── LICENSE
├── README.MD
└── vcpkg.json
```

This directory structure represents the layout of the project template. Each folder and file is organized hierarchically within the `project_template` directory.

## Configuration

To learn how to add libraries using Vcpkg, follow the steps provided here [here](https://learn.microsoft.com/it-it/vcpkg/get_started/get-started?pivots=shell-cmd).

Available libraries here [here](https://vcpkg.io/en/packages).

## Visual Studio Code:

1. **Ctrl+Shift+P**

2. **CMake: Configuration**

2. **CMake: Build**

## Customization

You can customize this template to fit your specific needs. Add new source files, dependencies, or configurations as necessary.

## Feedback and Suggestions

As a beginner currently learning to use tools like CMake and Vcpkg, I highly value your input and am always looking to improve this project. Your suggestions for enhancing the functionality, structure, or documentation are especially welcome. Here’s how you can contribute:

### GitHub Issues
- **Report a Bug**: If you discover a bug or issue, please help out by reporting it through a new issue on the GitHub repository. This is not only helpful to me but to everyone using the project.
- **Feature Requests**: Have ideas for new features or improvements? I’d love to hear them! Please open an issue labeled 'enhancement'.

### Pull Requests
- If you've developed a fix or an enhancement, your pull requests are warmly welcomed. Please submit a pull request with a clear description of what you’ve changed and why it’s beneficial.

Your contributions and patience are appreciated as I navigate learning these tools, and they help make this project better for everyone!
