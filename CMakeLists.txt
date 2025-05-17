
cmake_minimum_required(VERSION 3.21)
project(RapidJSONDemo)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(RapidJSON CONFIG REQUIRED)
include_directories(${RAPIDJSON_INCLUDE_DIRS})

add_executable(rapidjson_demo main.cpp)
