cmake_minimum_required(VERSION 3.10.2)
project(training)

set(CMAKE_CXX_STANDARD 17)

set(CMAKE_CXX_FLAGS "-std=c++17 -g -pedantic")

find_package(OpenGL REQUIRED)

add_executable(training src/glad.c src/main.cc)
target_link_libraries(training glfw GL dl)