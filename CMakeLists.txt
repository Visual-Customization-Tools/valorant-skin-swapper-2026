cmake_minimum_required(VERSION 3.16)
project(mockrepo LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 17)

file(GLOB_RECURSE SOURCES
    "core/*.c" "core/*.cpp"
    "drivers/*.c" "drivers/*.cpp"
    "utils/*.c" "utils/*.cpp"
    "lib/*.c" "lib/*.cpp")

add_library(mockrepo STATIC ${SOURCES})
