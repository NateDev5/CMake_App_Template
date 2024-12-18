cmake_minimum_required(VERSION 3.20)
project(CMake_Project)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(modules/example_module)

add_executable(CMake_Project src/main.cpp)

target_link_libraries(CMake_Project PRIVATE example_module)