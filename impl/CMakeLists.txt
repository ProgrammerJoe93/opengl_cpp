# CMake config
cmake_minimum_required(VERSION 3.20)

target_sources(opengl_cpp_lib STATIC
               inc/glad/glad.h
               inc/KHR/khrplatform.h
               src/glad.c
)

add_executable(opengl_cpp
               src/main.cpp
)

target_include_directories(opengl_cpp
    PRIVATE
        ${CMAKE_CURRENT_SOURCE_DIR}/src
)

target_link_libraries(opengl_cpp
    PRIVATE
        opengl_cpp_lib
)
