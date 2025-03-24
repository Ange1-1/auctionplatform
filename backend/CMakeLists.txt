cmake_minimum_required(VERSION 3.16)
project(Auctionplatform)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin)


# 添加子目录
add_subdirectory(src/auction)
