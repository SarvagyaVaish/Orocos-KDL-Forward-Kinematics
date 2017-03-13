cmake_minimum_required (VERSION 2.6)
project (FK_KDL_Tutorial)

find_package (orocos_kdl REQUIRED)
include_directories (${orocos_kdl_INCLUDE_DIRS})

add_executable (SimpleRobotFK main.cpp)
target_link_libraries (SimpleRobotFK ${orocos_kdl_LIBRARIES})
