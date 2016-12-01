cmake_minimum_required (VERSION 3.0)
project(umich_apriltags)

include_directories(${PROJECT_SOURCE_DIR}/apriltag-2016-10-21)

set(SOURCES_PATH ${PROJECT_SOURCE_DIR}/apriltag-2016-10-21/)

file(GLOB SOURCES ${SOURCES_PATH}*.c ${SOURCES_PATH}*.h  ${SOURCES_PATH}common/*.c ${SOURCES_PATH}common/*.h)

add_library(umich_apriltags ${SOURCES})
