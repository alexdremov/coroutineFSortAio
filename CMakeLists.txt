cmake_minimum_required(VERSION 3.17)
project(CoRoutines C)

set(CMAKE_C_STANDARD 11)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(CMAKE_C_FLAGS_DEBUG "-g3")
set(CMAKE_C_FLAGS_RELEASE  "-O0")
set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -lrt")

include_directories(.)
add_executable(coSortAio
        src/coSort.h
        src/coSort.c
        src/stack.c
        src/stack.h
        src/stackArrays.c
        src/stackArrays.h)
