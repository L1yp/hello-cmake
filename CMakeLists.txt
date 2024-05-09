cmake_minimum_required(VERSION 3.22.1)
project(hello_cmake)

set(CMAKE_CXX_STANDARD 11)

include_directories(interface src test)

aux_source_directory(src DIR_SRCS)

add_executable(hello_cmake
        test/Decoder.c
        ${DIR_SRCS}
)