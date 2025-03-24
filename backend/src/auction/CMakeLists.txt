# 收集 reactor 相关的核心源文件
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR}/../reactor CORE_SRC)

# 将所有 reactor 源文件添加到库
add_library(reactor ${CORE_SRC} AuctionServer.cpp)

# 添加可执行文件 auctionserver
add_executable(auctionserver auctionserver.cpp)

# 包含 reactor 目录中的头文件
include_directories(${CMAKE_SOURCE_DIR}/src/reactor)


# 链接 reactor 库以及系统线程库
target_link_libraries(auctionserver reactor  pthread)
