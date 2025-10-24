cmake_minimum_required(VERSION 3.10.0)

project(hello)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_executable(hello main.cpp)

find_package(fmt CONFIG REQUIRED)

target_link_libraries(hello PRIVATE fmt::fmt)