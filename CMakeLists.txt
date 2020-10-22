cmake_minimum_required(VERSION 3.4)

project(serialib)

add_library(serialib STATIC ./src/serialib.cpp)
target_include_directories(serialib
  PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include/
  PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/src/
  )
