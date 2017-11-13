CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(add_yan)


find_package(CUDA QUIET REQUIRED)

# Specify binary name and source file to build it from
CUDA_ADD_LIBRARY(add_yan Math.h Math.cpp add.cuh add.cu)
