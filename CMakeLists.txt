# cmake 最低版本需求
cmake_minimum_required(VERSION 2.8)

# 工程名称
project(cmake_study)

# 设置
set(CMAKE_CXX_STANDARD 11)

# 编译源码生成目标
add_executable(cmake_study src/main.cc)

install(TARGETS cmake_study DESTINATION bin)

enable_testing()
add_test(cmake_study_test cmake_study 12)