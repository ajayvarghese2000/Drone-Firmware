<p align="center">
	<a href="https://github.com/lboroWMEME-TeamProject/CCC-ProjectDocs"><img src="https://i.imgur.com/VwT4NrJ.png" width=650></a>
	<p align="center"> This repository is part of  a collection for the 21WSD001 Team Project. 
	All other repositories can be access below using the buttons</p>
</p>

<p align="center">
	<a href="https://github.com/lboroWMEME-TeamProject/CCC-ProjectDocs"><img src="https://i.imgur.com/rBaZyub.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/Dashboard"><img src="https://i.imgur.com/fz7rgd9.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/Cloud-Server"><img src="https://i.imgur.com/bsimXcV.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/Drone-Firmware"><img src="https://i.imgur.com/yKFokIL.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/Simulated-Drone"><img src="https://i.imgur.com/WMOZbrf.png" alt="drawing" height = 33/></a>
</p>

<p align="center">
	Below you can find buttons that link you to the repositories that host the code for the module itself. These can also be found linked in the collection repository: <a href="https://github.com/lboroWMEME-TeamProject/Drone-Firmware">Drone Firmware</a>. 
</p>


<p align="center">
	<a href="https://github.com/lboroWMEME-TeamProject/Main-Pi"><img src="https://i.imgur.com/4knNDhv.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/EnviroSensor"><img src="https://i.imgur.com/lcYUZBw.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/Geiger-Counter"><img src="https://i.imgur.com/ecniGik.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/Thermal-Camera"><img src="https://i.imgur.com/kuoiBTc.png" alt="drawing" height = 33/></a> 
	<a href="https://github.com/lboroWMEME-TeamProject/ai-cam"><img src="https://i.imgur.com/30bEKvR.png" alt="drawing" height = 33/></a>
</p>


------------

# Drone Firmware
This repo contains all the relevant repos, that hold the code for the individual subsystems that will be on the drone module.

The drone module is split as follows,
<div align="center">

||Description|Link|
|--|--|--|
| **Main-Pi** | The code base that will run on the main Raspberry Pi that handles data accusation from the individual sensors, packaging and sending of that data to the remote server. |[GitHub](https://github.com/lboroWMEME-TeamProject/Main-Pi) |
| **Geiger-Counter** | Code for Raspberry Pi Pico to get the sensor data from the Geiger counter  |[GitHub](https://github.com/lboroWMEME-TeamProject/Geiger-Counter) |
| **Enviro Sensor** | Code to operate and control the Enviro+ Sensor with a Raspberry Pi |[GitHub](https://github.com/lboroWMEME-TeamProject/EnviroSensor) |
| **Particulates Sensor** | Code to run get PPM values from the air as a measure of air quality |[GitHub](https://github.com/lboroWMEME-TeamProject/Particulates-Sensor)|
| **Ai-Cam** | Code to run the AI object detection on the raspberry Pi 4 and send its data to the Main Pi |[GitHub](https://github.com/lboroWMEME-TeamProject/ai-cam) |
| **Thermal-Cam** | Code to run and get images from the thermal camera |[GitHub](https://github.com/lboroWMEME-TeamProject/Thermal-Camera)|


</div>

------------

## Overview

**High Level Diagram:**

<p align="center">
	<img src="https://i.imgur.com/g5QJgSA.jpg" alt="drawing"/>
</p>

Each of the drone modules is connected to the central server via the use of websockets and streams the data to the server. 

The server then echo's the data back to the connected clients depending on what drone the client is connected to via normal HTTPS request.

There are a range on subsystems on the Drone Module itself each communicating and sending data to a central server running on a Raspberry Pi.

**Drone Module Level Diagram:**

<p align="center">
	<img src="https://i.imgur.com/8I0nU0g.jpg" alt="drawing"/>
</p>

All of the sub systems are attached to the 'Main-Pi', the Main Pi is connected to the outside world via WiFi to send the data it collects from the individual subsystems.

*To see the system breakdowns of the subsystems please visit their respective repos*
