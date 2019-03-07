cmake_minimum_required(VERSION 3.0)
project(tests)
file(GLOB TEST_FILES
        ../src/*.cpp
        ../src/*.h
        ../src/parser/bison_parser.cpp
        ../src/parser/bison_parser.h
        ../src/parser/flex_lexer.cpp
        ../src/parser/flex_lexer.h
        ../src/parser/parser_typedef.h
        ../src/parser/sql_keywords.txt
        ../src/util/*.cpp
        ../src/util/*.h
        ../src/sql/*.cpp
        ../src/sql/*.h
        *.cpp
        *.h
        queries/*
        thirdparty/microtest/microtest.h)
#include_directories(../src)
add_executable(${PROJECT_NAME} ${TEST_FILES})

