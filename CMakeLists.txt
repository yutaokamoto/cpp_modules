cmake_minimum_required(VERSION 3.0)

project(cpp_knapsack)
set(PYBIND11_CPP_STANDARD -std=c++14)
set(CMAKE_CXX_FLAGS "-Wall -Wextra -O2")
add_subdirectory(pybind11)

pybind11_add_module(cpp_knapsack SHARED cpp_knapsack.cpp)