
cmake_minimum_required(VERSION 3.14)
project(project_name VERSION 1.0 DESCRIPTION "Description of your project" LANGUAGES CXX)

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
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/src/utils)

# Create 'test' directory inside project directory
file(MAKE_DIRECTORY ${CMAKE_SOURCE_DIR}/tests)

# Find dependencies provided by vcpkg (via vcpkg.cmake)
find_package(fmt CONFIG REQUIRED)

# main target
add_executable(main)
target_sources(main PRIVATE src/core/main.cpp)
target_link_libraries(main PRIVATE fmt::fmt)
set_property(TARGET main PROPERTY CXX_STANDARD 23)

# tests target
#add_executable(tests)
#target_sources(tests PRIVATE test/test.cpp)
#target_link_libraries(tests PRIVATE fmt::fmt)
#set_property(TARGET tests PROPERTY CXX_STANDARD 23)
#enable_testing()
#add_test(tests tests)

