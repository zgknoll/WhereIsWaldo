cmake_minimum_required(VERSION 3.6)
project(WhereIsWaldo)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp Test.cpp Test.h)
add_executable(WhereIsWaldo ${SOURCE_FILES})

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )