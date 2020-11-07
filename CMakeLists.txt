cmake_minimum_required(VERSION 3.0)
project(cpython)

file(GLOB SOURCE_FILES
        Programs/*.c
        Python/*.c
        Parser/*.c
        Objects/*.c
        Modules/*.c)

include_directories(.)
include_directories(Include)

add_executable(python ${SOURCE_FILES})