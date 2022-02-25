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
<br><br>
<img src="https://raw.githubusercontent.com/ashtencodes/ashtencodes.github.io/master/images/d435i.gif" width="450">
<br><br>
<img src="https://user-images.githubusercontent.com/82536552/155690813-c2f6dc08-f108-4e45-9117-eb0092d37c4b.png" width="450">

# Motion Planning and Steering
Motion planning and perception here.

<br> <br>
<img src="https://user-images.githubusercontent.com/74911365/154952750-4908496f-8f39-4671-bfb4-977458b7e3d3.png" width="700">

<br> <br>
<img src="https://user-images.githubusercontent.com/74911365/155113519-014505a9-2f83-494c-89f7-714ab5776516.png">

# GPS Waypoint Navigation and ARUCO Tag Detection
GPS waypoint navigation and ARUCO.
<br><br>
![image](https://user-images.githubusercontent.com/74911365/155114147-ccfbe904-3fef-4b0c-9464-e95d38e2f24d.png)
<br><br>
Users can view, update, and delete reservations on their profile page.
<br><br>
![image](https://user-images.githubusercontent.com/74911365/155114317-cdf866ae-61aa-4f71-95c9-853912ff108a.png)

# Challenges And Accomplishments
The biggest challenge our team encountered was the management of large datasets across multiple local development platforms. Passing the necessary data to every corner of the project was difficult and clunky at first, but through a large-scale overhaul of our database and restructuring to use AJAX requests, we were able to clean up our code and easily access our database information. Another large accomplishment for the team was the sudden delve into web development. A majority of our team has little to no prior experience with web development, yet we were able to use this competition as an opportunity to jump in head first into new territory, which significantly accelerated our growth as programmers. We were able to learn more about web design, proper coding practices, and maximizing the use of version control systems.
