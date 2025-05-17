
cmake_minimum_required(VERSION 3.21)
project(RapidJSONDemo)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Find RapidJSON using MODULE mode instead of CONFIG mode
find_package(RapidJSON REQUIRED)

# Alternatively, we can directly use the vcpkg-installed headers
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/docker-ci/vcpkg/installed/x64-linux/include)

add_executable(rapidjson_demo main.cpp)
