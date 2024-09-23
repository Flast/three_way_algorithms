cmake_minimum_required(VERSION 3.11)

project(three_way_algorithms LANGUAGES CXX)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_MODULE_PATH "${CMAKE_MODULE_PATH};${CMAKE_SOURCE_DIR}")

enable_testing()

add_library(three_way_algorithms INTERFACE)
target_include_directories(three_way_algorithms INTERFACE .)

add_subdirectory(test)
