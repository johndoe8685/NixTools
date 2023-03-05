cmake_minimum_required(VERSION 3.0)

project(NixTools)

set(PROJECT_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/include)
set(PROJECT_SOURCE_DIR ${CMAKE_SOURCE_DIR}/src)

set(PROJECT_SOURCES
	${PROJECT_SOURCE_DIR}/directory.cpp
	${PROJECT_SOURCE_DIR}/debugger.cpp
	${PROJECT_SOURCE_DIR}/system.cpp
)

include_directories(${PROJECT_INCLUDE_DIR})
add_library(${PROJECT_NAME} STATIC ${PROJECT_SOURCES}) 