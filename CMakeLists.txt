cmake_minimum_required(VERSION 3.0)
project(umich_apriltags)

#add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/common)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/)

file(GLOB SOURCES *.c *.h  common/*.c common/*.h)
add_library(umich_apriltags ${SOURCES})
