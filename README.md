# Mesh Point Sampling
## Overview
**Author: [Igor Maurell], igormaurell@gmail.com**

The mesh_point_sampling software uses PCL to sample a point cloud in a mesh surface. This is pcl_mesh_sampling of pcl_tools with a modification to mantain the face information for each point.

## Dependencies
This software is implemented in C++ using the [Point Cloud Library](https://pointclouds.org) (PCL-1.10).

## Instalation
After install PCL-1.10, do:
    
    $ git clone --recursive https://github.com/igormaurell/mesh_point_sampling
    $ cd mesh_point_sampling
    $ mkdir build && cd build
    $ cmake ..
    $ make
    $ sudo make install

## Using
After install, use the help to understand the parameters, doing:
    
    $ mesh_point_sampling -h