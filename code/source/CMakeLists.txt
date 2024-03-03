# List of source files
set(SOURCE_FILES example.c)

# Create a static library
add_library(fscl-stm32xx-x STATIC ${SOURCE_FILES})

# Set include directories
target_include_directories(fscl-stm32xx-x PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

# Declare the dependency
add_dependencies(fscl-stm32xx-x fscl-stmxx-x-dep)

# Export the library as a dependency
add_library(fscl-stmxx-x-dep INTERFACE)
target_link_libraries(fscl-stmxx-x-dep INTERFACE fscl-stm32xx-x)
target_include_directories(fscl-stmxx-x-dep INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
