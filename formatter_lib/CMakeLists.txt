cmake_minimum_required(VERSION 3.4)
project(formatter)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
add_library(formatter_lib1 STATIC ${CMAKE_CURRENT_SOURCE_DIR}/formatter.cpp)
add_executable(formatter ${CMAKE_CURRENT_SOURCE_DIR}/formatter.cpp)
target_link_libraries(formatter formatter_lib1)
