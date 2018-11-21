cmake_minimum_required(VERSION 2.8.12)
project(opencv_examples)

add_definitions("-std=c++11")

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

add_executable(opencv_example main.cpp)
target_link_libraries(opencv_example ${CONAN_LIBS})
