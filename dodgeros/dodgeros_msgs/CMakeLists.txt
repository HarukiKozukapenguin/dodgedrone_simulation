cmake_minimum_required(VERSION 3.0.0)
project(dodgeros_msgs)

add_compile_options(-std=c++17)
add_compile_options(-O3)

find_package(catkin_simple REQUIRED 
roscpp
rospy
std_msgs
message_generation
)
catkin_simple(ALL_DEPS_REQUIRED)

#add_message_files(
#FILES
#VelCommand.msg
#)

#generate_messages(
#DEPENDENCIES
#std_msgs
#geometry_msgs
#)

cs_install()
cs_export()
