cmake_minimum_required(VERSION 2.8.3)
project(kraft_arm_msgs)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  message_generation
  std_msgs
  visualization_msgs
)

## Generate messages in the 'msg' folder
add_message_files(
 FILES
 ToolRequest.msg
 PoseRequest.msg
 CustomMarkerArray.msg
)

## Generate added messages and services with any dependencies listed here
generate_messages(
  DEPENDENCIES
  std_msgs
  geometry_msgs
)
