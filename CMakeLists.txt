# CMake config
cmake_minimum_required(VERSION 3.20)

# Project name
project(opengl_cpp)

# Language config
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Include
add_subdirectory(impl)
add_subdirectory(glfw)
