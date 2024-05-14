cmake_minimum_required(VERSION 3.0.0)
project(learnOpenGL VERSION 1.0.0)
cmake_policy(SET CMP0072 NEW)

find_package(OpenGL REQUIRED)

add_executable(learnOpenGL
        src/main.cpp
        src/glad.c
)

target_link_libraries(learnOpenGL
        glfw
        OpenGL::GL
)