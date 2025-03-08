cmake_minimum_required(VERSION 3.24)

project(test_ci VERSION 0.1
        DESCRIPTION "test_ci"
        LANGUAGES CXX)

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE "Release")
endif()

set(CMAKE_VERBOSE_MAKEFILE ON)

add_subdirectory(src)
add_subdirectory(tests)
