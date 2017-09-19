cmake_minimum_required(VERSION 3.7)
project(HW0_Square)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        glad/glad.c
        glad/glad.h
        glad/khrplatform.h
        Square.cpp)

set(LINKER_FLAGS "-lSDL2 -lSDL2main -lGL -ldl")
link_libraries("${LINKER_FLAGS}")
add_executable(HW0_Square ${SOURCE_FILES})