
cmake_minimum_required(VERSION 3.10)
project(RapidJSONDemo)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 查找 RapidJSON 的安装位置
# 方式1: 如果 RapidJSON 是通过包管理器安装的
find_package(RapidJSON QUIET)

# 添加可执行文件
add_executable(rapidjson_demo main.cpp)