cmake_minimum_required (VERSION 3.25)
project (DarkWorldServer)
set (CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_FLAGS "-std=c++20")
set(CMAKE_COLOR_DIAGNOSTICS ON)
file(GLOB_RECURSE sources src/**.cpp)
add_executable(DarkWorldServer
    ${sources}
)
include(cmake/CPM.cmake)
target_include_directories(DarkWorldServer PUBLIC
    src
)
