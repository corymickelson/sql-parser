file(GLOB SQLPARSER_SOURCE_FILES
        *.cpp
        parser/*.cpp
        sql/*.cpp
        util/*.cpp
        )
file(GLOB SQLPARSER_HEADER_FILES
        *.h
        parser/*.h
        sql/*.h
        util/*.h)
	
add_library(${PROJECT_NAME} ${SQLPARSER_SOURCE_FILES} ${SQLPARSER_HEADER_FILES})
add_library(dep::sqlparser ALIAS ${PROJECT_NAME})

target_include_directories(${PROJECT_NAME}
	PUBLIC 
	${PROJECT_SOURCE_DIR}/src)
