cmake_minimum_required(VERSION 3.10)
project(solver_lib LANGUAGES CXX)

add_library(solver_lib STATIC
    solver.cpp
    solver.h
)

