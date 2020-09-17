cmake_minimum_required(VERSION 3.10)

project(PatchMatchStereo)
option(DEBUG "debug mode" OFF)
set(CMAKE_CXX_FLAGS "-std=c++11")

if(DEBUG)
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O2 -g")
SET(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O2 -g")
endif()

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/PatchMatchStereo)
set(LIBRARY_OUTPUT_PATH "${CMAKE_CURRENT_SOURCE_DIR}/lib")
link_directories("${LIBRARY_OUTPUT_PATH}")

add_subdirectory(PatchMatchStereo) 
add_subdirectory(demo)
