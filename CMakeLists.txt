cmake_minimum_required(VERSION 3.25.0)
project(skia LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(Skia)
add_executable(TestDemo demo/main.cpp)
target_link_libraries(TestDemo skia)
