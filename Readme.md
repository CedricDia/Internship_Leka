This file contains part of what I was able to develop during my internship at leka. 
The code is opensource so I have no constraints.

I developed everything except this file :
LekaOS-cedric_lk_imu\drivers\CoreIMUlsm6dsox\extern



- **'/drivers'** contains a driver file which allows to interact with the inertial unit of the robot and retrieve his data.


- **'/libs/MotionKit'** contains libraries with the different variables and functions useful for the programs of the **'/spikes'** file.


- And the file **"/spikes"** contains programs that can be sent to the robot to serve as a test. 
Flashing a spike on the robot allows you to only launch it without being impacted by all the robot's features.

	• **'/spikes/lk_imu_app'** : The function of this program is to send data from the inertial unit at a certain frequency.
	At the same time, a process is launched which makes it possible to modify the frequency of sending via an RFID card

	Demo video: https://www.youtube.com/watch?v=0hk2X7VGsEY&ab_channel=C%C3%A9dricDiavorini


	• **'/spikes/lk_imu_mlc'**: the functions of this program are :
		◘ to read the data from the inertial unit via specific registers
		◘ to interpret the movement carried out by its decision tree integrated into the sensor 
		◘ to draw the shape obtained on the screen of the robot.

	Demo video: https://www.youtube.com/watch?v=bGj-rXCwy2c&ab_channel=C%C3%A9dricDiavorini