file(GLOB SOURCE_FILES
        *.cpp
        *.h
        parser/*.cpp
        parser/*.h
        sql/*.cpp
        sql/*.h
        util/*.cpp
        util/*.h)

add_library(${PROJECT_NAME} ${SOURCE_FILES})

