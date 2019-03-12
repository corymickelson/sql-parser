cmake_minimum_required(VERSION 3.0)
project(SQLPARSER_TEST)
file(GLOB TEST_FILES
        *.cpp
        *.h
        queries/*
        thirdparty/microtest/microtest.h)
set(CMAKE_BUILD_TYPE Debug)
add_executable(${PROJECT_NAME} ${TEST_FILES})
target_link_libraries(${PROJECT_NAME}
dep::sqlparser)
