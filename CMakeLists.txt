cmake_minimum_required(VERSION 3.22)

project(target)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(target main.c)
target_link_libraries(target ${SDL2_LIBRARIES})
set_property(TARGET target PROPERTY C_STANDARD 11)
