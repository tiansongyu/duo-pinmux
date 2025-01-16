cmake_minimum_required(VERSION 3.10)

# 项目信息
project(duo_pinmux C)

# 设置编译器

# 设置编译选项
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -static")

# 添加源文件
set(SOURCE_FILES duo_pinmux.c devmem.c)

# 添加可执行文件
add_executable(devmem ${SOURCE_FILES})

