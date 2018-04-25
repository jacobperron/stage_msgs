cmake_minimum_required(VERSION 2.8.3)
project(stage_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
)

################################################
## Declare ROS messages, services and actions ##
################################################

add_service_files(
  FILES
    SetClockInterval.srv
)

generate_messages()

catkin_package(
  CATKIN_DEPENDS
    message_runtime 
)
