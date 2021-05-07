cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

project(mesh_point_sampling)

find_package(PCL 1.10 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
include_directories(include)
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (mesh_point_sampling mesh_point_sampling.cpp include/point_types/point_types.h)
target_link_libraries (mesh_point_sampling ${PCL_LIBRARIES})