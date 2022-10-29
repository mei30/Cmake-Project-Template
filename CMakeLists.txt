cmake_minimum_required(VERSION 3.5)

project(cmake_template_project LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_INSTALL_PREFIX ${CMAKE_SOURCE_DIR})

message("ffffffffffffffffffff" ${CMAKE_SOURCE_DIR})

set(LIBRARY_INSTALL_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/include)
set(LIBRARY_INSTALL_BIN_DIR ${CMAKE_SOURCE_DIR}/bin)
set(LIBRARY_INSTALL_LIB_DIR ${CMAKE_SOURCE_DIR}/lib)

add_subdirectory(src)
