project(aerial-testbed)
cmake_minimum_required(VERSION 2.8)

set(SRC_DIR ${CMAKE_SOURCE_DIR}/src)

file(GLOB SOURCES ${SRC_DIR}/*.cpp)

add_executable(aerial-testbed ${SOURCES})

target_link_libraries(aerial-testbed kovan opencv_highgui opencv_core opencv_imgproc)

