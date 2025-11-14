cmake_minimum_required(VERSION 3.11)
project(EscPospp)

set(CMAKE_CXX_EXTENSIONS ON)
set(CMAKE_CXX_STANDARD 11)

file(GLOB SOURCES "src/*.cpp")

include_directories(./)

add_library(EscPospp ${SOURCES})
target_link_libraries(EscPospp usb-1.0)
target_include_directories(EscPospp PUBLIC ./)
