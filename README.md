# 3WheelRobotSample

1. This simulation is implemented using Coppelia Sim Edu software.
2. All the programs in the project are written in Lua programming language.

# Steps involved for creating the robot
Step-1:  The components are CAD files found online at https://roboticafaciles/coppeliasim/2Fdyor/2Fdyor-coppeliasim-files.zip

Step-2: Import all the models into the scene

<img width="326" alt="imports" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/42afafda-bba5-4ff9-92be-b3e7ef8fcb6a">


Step-3: Create pure shapes for **base, front, wheels, arms, caster wheel and caster support**

<img width="481" alt="shapes" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/1925a29b-8e66-4a32-a9fa-3826f93db41e">


Step-4: Group the extracted shapes as per the requirements like the following
  1. **Base and Front**
  2. **Arm joints and arm as shown in the image**
  3. **Caster support**

<img width="559" alt="grouped" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/4027554a-b32f-4ff3-ad5b-4688130f440b">


Step-5: Connect all the grouped and ungrouped shapes as following
  1. Connect the **Base** and **Arms** using revolute joints with Control Mode in **Position**
  2. Connect the **Base** and **Wheels** using revolote joints with Control Mode in **Velocity**
  3. Connect the **Base** and **Caster Support** using revolute joint with **Free** Control Mode
  4. Connect the **Caster Support** and **Caster Wheel** using revolute joint in **Free** mode.

<img width="477" alt="joints" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/0485f9a2-a63b-4328-b39d-a5297b72fabd">


Step-6: Re-design the **Scene Hierarchy** as follows

<img width="210" alt="shre1" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/97a6dfc9-36dc-4b0b-93bb-2dd714b4c20e">

<img width="181" alt="shre2" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/2df02da4-2ce6-49f1-93a6-41f674eac713">



Step-7: Place the proximity sensor at the sensor location and camera sensor at the bottom of the robot as shown

<img width="379" alt="proxi" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/b384b22c-0b89-40f1-ac80-a3cd5e6918f7">

<img width="134" alt="vision" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/d17d78a8-1bfc-4b53-92ee-828b9cfd490a">



Step-8: Find the code for the custom UI plugin in the file code.txt
The UI looks like this

<img width="221" alt="ui" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/0acee71a-5852-4207-9c0c-3d89827e9ddc">

Step-9: Create a wall around the robot for testing and learning about the sensor.
The toatal setup is like this

<img width="1280" alt="autonomousSetup" src="https://github.com/Veman-Mendu/3WheelRobotSample/assets/49408236/a065755a-2570-4091-a765-358f49bb94a2">

# Any ideas on making this project more complex, challenging and beautiful are appreiated and can be mailed to mvsprabhath17@gmail.com
