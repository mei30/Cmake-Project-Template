cmake_minimum_required(VERSION 3.2)
project(library C CXX)

set(SOURCE_FILES
	library.h
	library.cpp
)	

add_library(library STATIC SHARED ${SOURCE_FILES})

install(TARGETS library DESTINATION ${LIBRARY_INSTALL_LIB_DIR})
install(FILES library.h DESTINATION ${LIBRARY_INSTALL_INCLUDE_DIR})
