# Create the executable
add_executable(${PROJECT_NAME} main.c)

# Link the executable with the library created in inc
target_link_libraries(${PROJECT_NAME} PRIVATE ${PROJECT_NAME}Lib)
