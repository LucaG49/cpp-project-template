
cmake_minimum_required(VERSION 3.14)
project(project_name VERSION 1.0 DESCRIPTION "Description of your project" LANGUAGES CXX)

# Set compiler variables
set(CMAKE_C_COMPILER "C:/msys64/ucrt64/bin/gcc.exe")
set(CMAKE_CXX_COMPILER "C:/msys64/ucrt64/bin/g++.exe")
set(CMAKE_MAKE_PROGRAM "C:/msys64/ucrt64/bin/mingw32-make.exe")

# Find and use the fmt library
find_package(fmt CONFIG REQUIRED)

# Create 'build' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/build)

# Create 'docs' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/docs)

# Create 'include' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/include)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/include/core)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/include/gui)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/include/network)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/include/utils)

# Create 'lib' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/lib)

# Create 'resources' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/resources)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/resources/icons)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/resources/images)

# Create 'src' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/src/core)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/src/gui)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/src/network)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/src/tests)
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/src/utils)

# Create 'test' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/tests)

# Include directories
include_directories(${PROJECT_NAME} PRIVATE include)

# Add executable target
add_executable(${PROJECT_NAME} src/core/main.cpp)

# Link libraries
target_link_libraries(${PROJECT_NAME} PRIVATE fmt::fmt)

