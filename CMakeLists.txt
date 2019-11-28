cmake_minimum_required(VERSION 3.15)
project(untitled)

set(CMAKE_CXX_STANDARD 17)

include_directories(C:\\boost\\boost_1_71_0)
link_directories(C:\\boost\\boost_1_71_0\\stage\\lib)

find_package(Boost 1.71)
list(APPEND INCLUDE_DIRS ${BOOST_INCLUDE_DIRS})
list(APPEND LIBRARIES ${BOOST_LIBRARIES})

add_executable(untitled main.cpp)