#set(OpenCV_DIR /data/opencv342/share/OpenCV)
find_package(OpenCV REQUIRED)
if(NOT OpenCV_FOUND)
message(FATAL "opencv not found")
else()
message("found opencv libs: ${OpenCV_LIBS}")
endif()

include_directories(${OPENCV_INCLUDE_DIRS})

add_executable(demo main.cpp)

target_link_libraries(demo ${OpenCV_LIBS} pms)
