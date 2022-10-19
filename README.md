# Teaching_Robotics
################# DJI Tello ####################################
Ejecute los siguientes comandos:
	cd catkin_ws/src
  
	git clone https://github.com/anqixu/TelloPy.git
	cd TelloPy/
	sudo -H pip install -e .
	cd ..
	git clone https://github.com/anqixu/tello_driver.git
	git clone https://github.com/anqixu/h264_image_transport.git
	cd .. 
	rosdep install h264_image_transport
	pip install av
	catkin_make

pip install pyyaml

====================================================
Ejecución Tello
====================================================

primera terminal 

roscore

segunda terminal 

cd ~/catkin_ws
roslaunch tello_driver tello_node.launch

tercera terminal

cd ~/catkin_ws
roslaunch keyboard dji_tello_keyboard.launch
