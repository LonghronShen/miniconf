cmake_minimum_required(VERSION 3.0)

project(miniconf-examples)

set(EX1_SRC "miniconf_example1.cpp")
set(EX2_SRC "miniconf_example2.cpp")

add_executable(miniconf_example1 ${EX1_SRC})

target_link_libraries(miniconf_example1
    PUBLIC miniconf)

add_executable(miniconf_example2 ${EX2_SRC})

target_link_libraries(miniconf_example2
    PUBLIC miniconf)