cmake_minimum_required(VERSION 3.22.1)
project(shimmer)

add_library(shimmer SHARED native-lib.cpp)
find_library(log-lib log)
target_link_libraries(shimmer ${log-lib})