cmake_minimum_required(VERSION 3.10)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# set the project name
project(Project)

add_executable(Project tutorial.cpp)

# add the Sources library
add_subdirectory(Sources)

target_include_directories(Project PUBLIC
                          "${PROJECT_SOURCE_DIR}/Sources"
                          )