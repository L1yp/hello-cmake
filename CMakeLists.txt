cmake_minimum_required(VERSION 3.28)
project(hello_cmake)

set(CMAKE_CXX_STANDARD 11)

include_directories(interface src test)

add_executable(hello_cmake
        test/Decoder.c
)
