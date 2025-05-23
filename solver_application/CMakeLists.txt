cmake_minimum_required(VERSION 3.10)
project(solver LANGUAGES CXX)

add_executable(solve
    equation.cpp
)

target_include_directories(solve
    PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}/../formatter_ex_lib
    ${CMAKE_CURRENT_SOURCE_DIR}/../solver_lib
)

target_link_libraries(solve
    PRIVATE
    formatter_ex
    solver_lib
)
