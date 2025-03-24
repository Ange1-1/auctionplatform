# 收集所有源文件
aux_source_directory(${CMAKE_CURRENT_SOURCE_DIR} REACTOR_SRC)

# 创建静态库 reactor
add_library(reactor STATIC ${REACTOR_SRC})
