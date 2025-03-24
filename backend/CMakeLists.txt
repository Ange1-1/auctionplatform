cmake_minimum_required(VERSION 3.16)
project(AuctionPlatform)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 设置可执行文件的输出路径
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin)

# 添加子目录
add_subdirectory(src/reactor)    # 网络库
add_subdirectory(src/auction)    # 竞拍逻辑
add_subdirectory(src/main)       # 主程序入口
