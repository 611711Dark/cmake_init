# cmake version
cmake_minimum_required(VERSION 3.31.3)
# project name
project(cmake_init)

# set c++ version
set(CMAKE_CXX_STANDARD 17)

# include dir add,split by<space>
# include_directories()

# link dir add
# link_directories()

# add source
aux_source_directory(./src DIR_SRCS)
add_executable(cmake_init ${DIR_SRCS})

