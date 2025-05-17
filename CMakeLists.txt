
cmake_minimum_required(VERSION 3.21)
project(RapidJSONDemo)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(RapidJSON CONFIG REQUIRED)

add_executable(rapidjson_demo main.cpp)

# RapidJSON is a header-only library, so we only need to include its directories
target_include_directories(rapidjson_demo PRIVATE ${RAPIDJSON_INCLUDE_DIRS})
