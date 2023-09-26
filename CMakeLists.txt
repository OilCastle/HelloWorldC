# CMake minimum version required
cmake_minimum_required(VERSION 3.22)

# Project name and version
project(
    HelloWorld
    VERSION 1.0
    DESCRIPTION "Cpp Test"
    LANGUAGES C)

# Project C/Cpp standard set
set(CMAKE_C_STANDARD 23)
set(CMAKE_CXX_STANDARD 23)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -g")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g")

# Add the subdirectories
add_subdirectory(inc)
add_subdirectory(src)

# Project target set
set(OUTPUT_DIR ${CMAKE_CURRENT_LIST_DIR}/build)
set_target_properties(${PROJECT_NAME} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${OUTPUT_DIR})
