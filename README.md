YOLO for ROS on Jetson

This is darknet ROS for Nvidia Jetson.
cd ~/catkin_ws>catkin_make   #Build

$ source ./devel/setup.bash

$ roscore

$ rosrun usb_cam usb_cam_node /usb_cam/image_raw:=/camera/image_raw

$ roslaunch darknet_ros darknet_ros.launch

$ rosrun rqt_graph rqt_graph

# usb 카메라가 darknet_ros에 날리는구나  카메라 row를 요청하니 계속 주고 있구나...

$ rqt_graph

$rviz

$rostopic list  
#darknet_ros/bounding_boxes 쓸만하다.
