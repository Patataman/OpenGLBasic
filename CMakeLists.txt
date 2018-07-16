cmake_minimum_required(VERSION 3.1)
project(OpenGL)

set(SRC_DIR "${CMAKE_CURRENT_SOURCE_DIR}")

#Compile window.cpp
set(SOURCES "${SRC_DIR}/window.cpp")

#Files to compile
add_executable(${PROJECT_NAME} ${SOURCES})

#Where search for headers
target_include_directories(${PROJECT_NAME} PRIVATE "${SRC_DIR}/include")

#Use C++11
set_property(TARGET ${PROJECT_NAME} PROPERTY CXX_STANDARD 11)