# 收集所有源文件
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} AUCTION_SRC)

# 创建静态库 auction
add_library(auction STATIC ${AUCTION_SRC})

# 包含头文件
target_include_directories(auction PUBLIC ${CMAKE_SOURCE_DIR}/src/reactor)

# 链接 reactor 库
target_link_libraries(auction PUBLIC reactor)
