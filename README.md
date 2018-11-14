In order to load a Turtlebot3 model with a camera there are minor changed that needs to be added to the urdf files. This repository includes the files ready with the needed additions. 
In order to use them please do the following:

1. Download the turtlebot3 package from the turtlebot3 repository to your workspace
2. Copy both the *.xacro files into: <your workspace>/src/turtlebot3/turtlebo3_description/urdf
3. Copy the launch file into the launch directory in your own package (if you don't have one, please create it)
4. Notice the gazebo launch launches an empty world. if you want to run a different world change the path under "world name" according to the world file you want to use.

The changes done to the files mostly include: 
* adding a camera link to the .urdf.xacro file
* a refrence to the .gazebo.xacro file, which includes a gazebo camera plugin
* a path to the new .urdf file in the launch file under description. 
