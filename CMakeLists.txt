cmake_minimum_required(VERSION 3.0.2)
project(ben_description)

find_package(catkin REQUIRED COMPONENTS
  xacro
  usv_gazebo_plugins
)

catkin_package(
  CATKIN_DEPENDS xacro usv_gazebo_plugins
)
