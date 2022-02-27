---
layout: post
author: Ashten Akemoto
---
# Robotic Space Exploration Lab
The Robotic Space Exploration Lab (RoSE) is an undergraduate and graduate student led research lab at the University of Hawaii studying space exploration and research applications in robotics! The projects range from studying rover terramechanics to machine learning powered celestial navigation and satellite development.

As a Software Engineer and Integrator for [VIP RoSE](http://www.uhmviprose.com/), I design, develop, test, and deploy a navigation stack providing our mars rover with autonomous navigation capabilities. Many subsystems consisting of over 30 students contribute to a single rover designed to compete at the [University Rover Challenge](https://urc.marssociety.org/home), a international collegiate robotics competition.

# Autonomous Traversal Mission
Summarized briefly, the autonomous travel mission requires the rover to navigate across extreme terrain and untraversable obstacles in the desserts of Hanksville, Utah, a similar environment to the martian surface. The rover must navigate to predetermined GPS waypoints, search and drive to scattered AR tags, and drive through gates without the intervention of a human operator. As a software engineer in the autonomy team, I integrate the **localization, percpetion, planning, and control** functionalities critical for the mission's success. 
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155688438-9665ee59-25b7-4984-b313-53130ccb8c56.png" width="900">

# Perception, Sensors, and SLAM
I have tested and integrated hardware components necessary for the navigation for the rover, such as GPS for localization, IMU (Inertial Measurement Unit) for orientation and acceleration data, and stereo cameras used for depth perception. Working with hardware wrappers and visualization tools, I integrated our hardware sensors into the **Robotic Operating System** (ROS) environment for easy integration with other modules. 
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155689625-65d42043-1c4a-4324-8617-19126de58075.png" width="900">
<div align="center">
  <i>Testing and validation of GPS precision functional requirement.</i>
</div>
<br><br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/d435i.gif" width="550">
<div align="center">
  <i>Outdoor testing clip of Intel d435i Stereo Camera.</i>
</div>
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155690813-c2f6dc08-f108-4e45-9117-eb0092d37c4b.png" width="550">
<div align="center">
  <i>Validation of depth sensing field of view functional requirement.</i>
</div>


Utilizing an open-source SLAM (Simultaneous Localization and Mapping) program called ORB-SLAM 3, the rover is able to localize and map its environment!
<br> <br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/mapping.gif" width="700">
<div align="center">
  <i>SLAM visualization of hallway and staircase using Rtabmap.</i>
</div>

# Simulations: Motion Planning & Steering
In the project, I led the development of the **motion planning and steering of the rover**. **Motion planning** entails generating the best path to avoid all obstacles and untraversable terrain, and is made possible through the move_base package. **Steering** is the process of creating and sending motion commands to fulfill the desired path of the rover. **I have created a fully fleshed out simulation of an autonomous rover in the ROS physics simulator, Gazebo**! I have integrated ackermann steering and skid-steering into different custom robot models fully equppied with simulated sensors. From detecting obstacles to generating and fulfilling a desired path, the simulation acts as a testbed and verifies our software components before integration into the competition chassis.
<br> <br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/ackermann.gif" width="450">
<div align="center">
  <i>Teleoperation of simulated ackermann vehicle using ros_controller in Gazebo.</i>
</div>

<br> <br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/obstacles.gif" width="700">
<div align="center">
  <i>Simulated skid-steering rover detecting and avoiding obstacles.</i>
</div>

<br> <br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/terrain.gif" width="700">
<div align="center">
  <i>Navigation through recognizition of untraversable terrain.</i>
</div>

# GPS Waypoint / ARUCO Tag Detection
The GPS waypoint navigation module is another one of my contributions. The waypoint module acts as an **interface to send GPS coordinate goals to the navigation stack**. The module takes in a goal latitude and longitude value and reads the current latitude and longitude to compute a vector from the rover's coordinate to the goal coordinate. In the competition, this node is necessary to send the goal GPS points to our autonomous navigation stack to be fulfilled by move_base!

<img src="https://user-images.githubusercontent.com/82536552/155824730-8df02370-313e-4e60-9d98-96f666aef670.png" width="650">

The ARUCO tag detection module detects AR tags from the video feed of our stereo camera. With the AR tags having a preset size, the module is able to calculate the position and orientation of the tag with respect to the rover and is able to a generate a similar vector to be sent to the navigation stack. This allows the rover to follow tags around!
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155697730-1409f81c-2956-49a0-adca-385c73665844.png" width="550">
<div align="center">
  <i>Demonstration of ARUCO tag detection module at ~10 meters distance.</i>
</div>


# Challenges And Accomplishments
Working on the autonomous rover team has introduced me to the world of robotics and software engineering. Difficult problems in autonomous robotics such as localization, perception, and navigation have no concrete "best" solutions, and our implementation of various modules and packages is unique to our navigation stack. Yet, in a little more than a semester, our team has been able to develop a pipeline of functionality ranging from hardware components to software algorithms that make autonomous navigation possible. On the software engineering end, I have learned valuable skills ranging from **software design decisions, programming best practices, and utilizing version control for issue driven development**. From rigorous testing of components to validation of functional requirements, I work in a hands-on and fast-paced engineering project alongside an extraordinarily talented team to further my skills in robotics and software engineering.
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155701223-c9702c5d-014b-4e5a-8ccc-a564300b5ec0.png" width="900">
