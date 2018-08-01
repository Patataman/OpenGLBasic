cmake_minimum_required(VERSION 3.1)

set(SRC_DIR "${CMAKE_CURRENT_SOURCE_DIR}")

#Compile window.cpp
add_executable(window "${SRC_DIR}/window.cpp")
#Compile other.cpp
add_executable(other "${SRC_DIR}/other.cpp")

#Where search for headers
include_directories(PRIVATE "${SRC_DIR}/include")

#Use C++11
set_property(GLOBAL PROPERTY CXX_STANDARD 11)
