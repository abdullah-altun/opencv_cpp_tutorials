cmake_minimum_required(VERSION 3.10)
project(OpenCVProject)

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})


add_executable(ImageRead src/imageRead.cpp)
add_executable(Example2 src/example2.cpp)

target_link_libraries(ImageRead ${OpenCV_LIBS})
target_link_libraries(Example2 ${OpenCV_LIBS})


