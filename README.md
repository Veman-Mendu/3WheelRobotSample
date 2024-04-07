# 3WheelRobotSample

1. This simulation is implemented using Coppelia Sim Edu software.
2. All the programs in the project are written in Lua programming language.

# Steps involved for creating the robot
Step-1:  The components are CAD files found online at https://roboticafaciles/coppeliasim/2Fdyor/2Fdyor-coppeliasim-files.zip

Step-2: Import all the models into the scene

Step-3: Create pure shapes for **base, front, wheels, arms, caster wheel and caster support**

Step-4: Group the extracted shapes as per the requirements like the following
  1. **Base and Front**
  2. **Arm joints and arm as shown in the image**
  3. **Caster support**

Step-5: Connect all the grouped and ungrouped shapes as following
  1. Connect the **Base** and **Arms** using revolute joints with Control Mode in **Position**
  2. Connect the **Base** and **Wheels** using revolote joints with Control Mode in **Velocity**
  3. Connect the **Base** and **Caster Support** using revolute joint with **Free** Control Mode
  4. Connect the **Caster Support** and **Caster Wheel** using revolute joint in **Free** mode.

Step-6: Re-design the **Scene Hierarchy** as follows

Step-7: Place the proximity sensor at the sensor location and camera sensor at the bottom of the robot as shown

Step-8: Find the code for the custom UI plugin in the file code.txt
