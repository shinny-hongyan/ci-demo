
cmake_minimum_required(VERSION 3.10)
project(RapidJSONDemo)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(RapidJSON CONFIG REQUIRED)
target_link_libraries(rapidjson_demo PRIVATE RapidJSON rapidjson)

# 添加可执行文件
add_executable(rapidjson_demo main.cpp)