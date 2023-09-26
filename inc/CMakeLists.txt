# This creates a library from the header files
add_library(${PROJECT_NAME}Lib INTERFACE)
target_include_directories(${PROJECT_NAME}Lib INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
