find_package(OpenCV)

include_directories(${OPENCV_INCLUDE_DIRS})

add_executable(demo main.cpp)

target_link_libraries(demo ${OpenCV_LIBS} pms)