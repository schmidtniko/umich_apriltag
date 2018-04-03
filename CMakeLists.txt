cmake_minimum_required(VERSION 3.0)
project(umich_apriltags)

file(GLOB SOURCES *.c *.h  common/*.c common/*.h)
add_library(umich_apriltags ${SOURCES})
target_include_directories(umich_apriltags PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
