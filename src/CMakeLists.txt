cmake_minimum_required(VERSION 3.2)
project(cmake_template C CXX)

add_subdirectory(library)

add_executable(cmake_template main.cpp)

target_include_directories(cmake_template PRIVATE library)

target_link_libraries(cmake_template library)

install(TARGETS cmake_template DESTINATION ${LIBRARY_INSTALL_BIN_DIR})


