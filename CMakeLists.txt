cmake_minimum_required(VERSION 3.14)

project(tcpshm )

option(test "Build all tests" ON)

enable_testing()

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -D_GLIBCXX_USE_CXX11_ABI=0")



add_subdirectory("test")
