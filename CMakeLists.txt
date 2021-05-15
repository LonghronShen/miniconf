cmake_minimum_required(VERSION 3.0)

project(miniconf-project)

option(MINICONF_BUILD_EXAMPLES "Build examples for miniconf" ON)

add_subdirectory(src)

if(MINICONF_BUILD_EXAMPLES)
    add_subdirectory(examples)
endif()