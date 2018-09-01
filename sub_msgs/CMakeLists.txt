cmake_minimum_required(VERSION 2.8.3)
project(sub_msgs)

find_package(catkin REQUIRED message_generation)

add_message_files(
  FILES
  Sub.msg
)

generate_messages(
)

catkin_package(
  CATKIN_DEPENDS message_runtime
)

