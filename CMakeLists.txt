cmake_minimum_required(VERSION 2.8.3)
project(mas_qt_tablet_interface)

find_package(catkin REQUIRED COMPONENTS
    rospy
)

catkin_package(
  CATKIN_DEPENDS
    rospy
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

install(DIRECTORY ros/launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)
