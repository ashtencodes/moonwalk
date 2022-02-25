---
layout: post
author: Ashten Akemoto
---
# Robotic Space Exploration Lab
The Robotic Space Exploration Lab (RoSE) is an undergraduate and graduate student led research lab at the University of Hawaii studying space exploration and research applications in robotics! Our projects range from studying rover terramechanics to machine learning powered celestial navigation and satellite development.

As a Software Engineer and Integrator for [VIP RoSE](http://www.uhmviprose.com/), I design, develop, test, and deploy a navigation stack providing our mars rover with autonomous navigation capabilities. Many subsystems consisting of over 30 students contribute to a single rover designed to compete at the [University Rover Challenge](https://urc.marssociety.org/home), a international collegiate robotics competition.

# Autonomous Traversal Mission
Summarized briefly, the autonomous travel mission requires the rover to navigate across extreme terrain and untraversable obstacles in the desserts of Hanksville Utah, a similar environment to the martian surface. The rover must navigate to predetermined GPS waypoints, search and drive to scattered AR tags, and drive through gates without the intervention of a human operator. As a software engineer in the autonomy team, I integrate the **localization, percpetion, planning, and control** functionalities critical for the mission's success. 
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155688438-9665ee59-25b7-4984-b313-53130ccb8c56.png" width="900">

# Perception, Sensors, and SLAM
I have tested and integrated hardware components necessary for the navigation for the rover, such as GPS for localization, IMU (Inertial Measurement Unit) for orientation and acceleration data, and stereo cameras used for depth perception. Working with hardware wrappers and visualization tools, I integrated our hardware sensors into the **Robotic Operating System** (ROS) environment for easy integration with other modules. 
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155689625-65d42043-1c4a-4324-8617-19126de58075.png" width="900">
Testing and validation of GPS precision functional requirement.
<br><br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/d435i.gif" width="450">
Outdoor testing clip of Intel d435i Stereo Camera.
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155690813-c2f6dc08-f108-4e45-9117-eb0092d37c4b.png" width="450">
Validation of depth sensing field of view functional requirement.

Utilizing an open-source SLAM (Simultaneous Localization and Mapping) program called ORB-SLAM 3, the rover is able to localize and map its environment!

# Motion Planning and Steering
In the project, I led the development of the motion planning and steering of the rover. Motion planning entails generating the best path to avoid all obstacles and untraversable terrain, and is made possible through the move_base package. Steering is the process of creating and sending motion commands to fulfill the desired path of the rover. I have integrated both ackermann steering and skid steering into a simulated autonomous rover built in the ROS simulation program, Gazebo! From detecting obstacles to generating and fulfilling a desired path, the simulation acts as a testbed and verifies our software components before integration into the competition chassis.

<br> <br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/ackermann.gif" width="450">

# GPS Waypoint Navigation and ARUCO tag detection
The GPS waypoint navigation module is another one of my contributions. The waypoint module acts as an interface to send GPS coordinate goals to the navigation stack. The module takes in a goal latitude and longitude value and reads the current latitude and longitude to compute a vector from the rover's coordinate to the goal coordinate. In the competition, this node is necessary to send the goal GPS points to our autonomous navigation stack to be fulfilled by move_base!

<br><br>
![image](https://user-images.githubusercontent.com/74911365/155114147-ccfbe904-3fef-4b0c-9464-e95d38e2f24d.png)

The ARUCO tag detection module detects AR tags from the video feed of our stereo camera. With the AR tags having a preset size, the module is able to calculate the position and orientation of the tag with respect to the rover and is able to a generate a similar vector to be sent to the navigation stack. This allows the rover to follow tags around!

# Challenges And Accomplishments
The biggest challenge our team encountered was the management of large datasets across multiple local development platforms. Passing the necessary data to every corner of the project was difficult and clunky at first, but through a large-scale overhaul of our database and restructuring to use AJAX requests, we were able to clean up our code and easily access our database information. Another large accomplishment for the team was the sudden delve into web development. A majority of our team has little to no prior experience with web development, yet we were able to use this competition as an opportunity to jump in head first into new territory, which significantly accelerated our growth as programmers. We were able to learn more about web design, proper coding practices, and maximizing the use of version control systems.
