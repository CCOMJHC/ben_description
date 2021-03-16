cmake_minimum_required(VERSION 3.0.2)
project(ben_description)

find_package(catkin REQUIRED COMPONENTS
  xacro
)

if(NOT EXISTS ${PROJECT_SOURCE_DIR}/models/meshes/BEN_shell.dae)
  execute_process(COMMAND gunzip -k ${PROJECT_SOURCE_DIR}/models/meshes/BEN_shell.dae.gz)
endif()

catkin_package(
  CATKIN_DEPENDS xacro
)
