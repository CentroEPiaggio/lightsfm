cmake_minimum_required(VERSION 3.0.2)
project(lightsfm)

add_compile_options(-std=c++11)

find_package(catkin REQUIRED COMPONENTS)

catkin_package(
  INCLUDE_DIRS include
)

install(
  DIRECTORY include/
  DESTINATION ${CATKIN_PACKAGE_INCLUDE_DESTINATION}
)
