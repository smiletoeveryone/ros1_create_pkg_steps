# ros_create_pkg_steps

Creating a ROS Package
http://wiki.ros.org/ROS/Tutorials/CreatingPackage
### You should have created this in the Creating a Workspace

### Tutorial
$ cd ~/catkin_ws/src

$ catkin_create_pkg beginner_tutorials std_msgs rospy roscpp

$ cd ~/catkin_ws

$ catkin_make

$ . ~/catkin_ws/devel/setup.bash

### package dependencies
$ rospack depends1 beginner_tutorials

$ rospack depends1 rospy

$ rospack depends beginner_tutorials

### Writing a Simple Publisher and Subscriber (C++)

http://wiki.ros.org/ROS/Tutorials/WritingPublisherSubscriber%28c%2B%2B%29

roscd beginner_tutorials

mkdir -p src

### Examining the Simple Publisher and Subscriber

### ***Follow all steps as the website

http://wiki.ros.org/ROS/Tutorials/ExaminingPublisherSubscriber

1. Running the Publisher

$ roscore

### In your catkin workspace

$ cd ~/catkin_ws

$ source ./devel/setup.bash

$ rosrun beginner_tutorials talker (C++)

$ rosrun beginner_tutorials talker.py (Python)

2. Running the Subscriber

$ rosrun beginner_tutorials listener (C++)

$ rosrun beginner_tutorials listener.py (Python)
