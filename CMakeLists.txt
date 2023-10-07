cmake_minimum_required(VERSION 3.21)
project(opencv_learn)

set(CMAKE_CXX_STANDARD 17)

find_package(OpenCV REQUIRED)
find_package(GFLAGS REQUIRED)
find_package(Eigen3 REQUIRED)

message(STATUS "OpenCV_INCLUDE_DIRS: ${OpenCV_LIBRARIES}")

include_directories(
        ${OpenCV_INCLUDE_DIRS}
        ${GFLAGS_INCLUDE_DIR}
        ${EIGEN3_INCLUDE_DIR}
)

link_libraries(
        ${GFLAGS_LIBRARIES}
        ${OpenCV_LIBRARIES}
)




