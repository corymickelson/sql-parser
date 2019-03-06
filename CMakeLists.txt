cmake_minimum_required(VERSION 3.13)
project(sql_parser)

set(CMAKE_CXX_STANDARD 14)

set(CMAKE_CXX_FLAGS_DEBUG "-g")
set(CMAKE_CXX_FLAGS_RELEASE "-O3")


add_subdirectory(src)
add_subdirectory(test)

