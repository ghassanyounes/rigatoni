cmake_minimum_required(VERSION 3.23)
project(rigatoni)

include(FindPkgConfig)
find_package(waylandpp)

set(CMAKE_CXX_STANDARD 20)

add_compile_options(-g)

add_executable(rigatoni main.cpp)
target_link_libraries(rigatoni ${waylandpp_LIBRARIES})
