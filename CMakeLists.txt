cmake_minimum_required(VERSION 2.8)
project(aoc2017)

SET(CMAKE_CXX_COMPILER clang++)
SET(CLANG_COMPILE_FLAGS "-Wall -Wextra -Wfatal-errors --std=c++14 -g")
SET(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} ${CLANG_COMPILE_FLAGS}" )

#Find all cpp files recursively
file(GLOB_RECURSE SRC "src" "src/*.cpp")

add_executable(aoc ${SRC})
target_link_libraries(aoc)
