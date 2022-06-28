cmake_minimum_required(VERSION 3.17)
project(rtp C)
set(CMAKE_C_STANDARD 99)
include(CMakeDependentOption)

# need delete cmake-build-*
CMAKE_DEPENDENT_OPTION(ENABLE_TEST "enable test" ON "${CMAKE_SOURCE_DIR} STREQUAL ${CMAKE_CURRENT_SOURCE_DIR}" OFF)


add_subdirectory(rtp)
