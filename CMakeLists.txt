cmake_minimum_required(VERSION 3.28 FATAL_ERROR)
project(real_world_units)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(real_world_units INTERFACE)
add_library(Physics::Units ALIAS real_world_units)

target_include_directories(real_world_units INTERFACE include)

option(BUILD_TESTING "Build tests" ON)

if(BUILD_TESTING AND EXISTS "${CMAKE_CURRENT_SOURCE_DIR}/test/CMakeLists.txt")
  add_subdirectory(test)
endif()
