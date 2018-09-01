cmake_minimum_required(VERSION 2.8.3)
project(helloworld_rosjava_messages)

find_package(catkin REQUIRED rosjava_build_tools rosjava_bootstrap genjava helloworld_msgs)

generate_rosjava_messages(
  PACKAGES
    helloworld_msgs
)

catkin_package()
