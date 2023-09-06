cmake_minimum_required(VERSION 3.21)

project(Dipinto)

if (NOT DEFINED CMAKE_CXX_STANDARD)
    set(CMAKE_CXX_STANDARD 20)
endif()

include(../Common/CMake/PreventInSourceBuilds.cmake)
include(../Common/CMake/CompilerWarnings.cmake)

add_executable(Dipinto main.cpp)
cmtools_set_compiler_warnings(Dipinto TRUE "" "" "" "")
