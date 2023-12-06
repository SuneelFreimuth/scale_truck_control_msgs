cmake_minimum_required(VERSION 2.8.3)
project(scale_truck_control_msgs)

find_package(catkin REQUIRED
  COMPONENTS
    message_generation
)

add_message_files(
  DIRECTORY msg
  FILES
    lane_coef.msg
    lane.msg
    xav2lrc.msg
    lrc2xav.msg
    lrc2ocr.msg
    ocr2lrc.msg
)

generate_messages()

catkin_package(
  CATKIN_DEPENDS
    message_runtime
)

