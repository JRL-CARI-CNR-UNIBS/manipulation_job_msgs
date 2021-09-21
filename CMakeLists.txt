cmake_minimum_required(VERSION 3.0.2)
project(manipulation_jobs_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
)



find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  message_generation
  std_msgs
  control_msgs
  sensor_msgs
  actionlib
  actionlib_msgs
)

add_message_files(
  FILES
  )

add_service_files(
  FILES
  ListOfExecuterProperties.srv
  )

add_action_files(
  FILES
)

generate_messages(
  DEPENDENCIES
  geometry_msgs std_msgs actionlib_msgs control_msgs sensor_msgs
)

catkin_package(
)
