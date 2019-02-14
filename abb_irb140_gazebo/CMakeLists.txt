cmake_minimum_required(VERSION 2.8.3)
project(abb_irb140_gazebo)

## Compile as C++11, supported in ROS Kinetic and newer
# add_compile_options(-std=c++11)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED)


catkin_package(
)

foreach(dir config launch urdf)
   install(DIRECTORY ${dir}/
      DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach()

install(FILES readme.md DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

