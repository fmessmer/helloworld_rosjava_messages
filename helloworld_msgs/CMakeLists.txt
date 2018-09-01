cmake_minimum_required(VERSION 2.8.3)
project(helloworld_msgs)

find_package(catkin REQUIRED message_generation actionlib_msgs sub_msgs)

add_action_files(
  FILES
  HelloWorld.action
  HelloWorldSub.action
)

generate_messages(
  DEPENDENCIES
  actionlib_msgs
  sub_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime actionlib_msgs sub_msgs
)

