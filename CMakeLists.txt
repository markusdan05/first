cmake_minimum_required(VERSION 4.2.0)

project(First)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/out/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/out/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/out/bin)

include_directories(
	./src/inc/
)

add_executable(${PROJECT_NAME}
	./src/main.cpp
	./src/inc/a.h
	./src/inc/a.cpp
)