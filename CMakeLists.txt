# CMake starter for C++17

cmake_minimum_required( VERSION 3.0 )
project( project_name CXX )

# Set Environment variables used by CMAke.
set( CMAKE_CXX_STANDARD 17 )
set( CMAKE_CXX_STANDARD_REQUIRED ON )
set( CMAKE_CXX_FLAGS "-Wall -Wextra" )  
set( CMAKE_BUILD_TYPE Debug )

# Set the source file. 
# Multiple source files can be included with a space .
set( SRCS src/Source.cpp )

# include directories for the include folder and libraries folder.
include_directories( $(include/) )
include_directories( $(lib/) )

# add source files to the project.
add_executable( project_name ${SRCS} )