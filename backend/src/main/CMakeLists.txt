# 创建可执行文件 auctionserver
add_executable(auctionserver auctionserver.cpp)

# 包含头文件
target_include_directories(auctionserver PRIVATE ${CMAKE_SOURCE_DIR}/src/auction )

# 链接 reactor 和 auction 库
target_link_libraries(auctionserver PRIVATE reactor auction pthread)
