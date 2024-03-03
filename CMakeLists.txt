cmake_minimum_required(VERSION 3.0.0)
project(STM32xx_Template C CXX)

# Set C and C++ standards
set(CMAKE_C_STANDARD 99)
set(CMAKE_CXX_STANDARD 11)

# Enable treat warnings as errors
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Werror")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Werror")

# Add the 'code' subdirectory
add_subdirectory(code)
