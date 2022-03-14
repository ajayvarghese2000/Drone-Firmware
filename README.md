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

------------

# Drone Firmware
This repo contains all the relevant repos, that hold the code for the individual subsystems that will be on the drone module.

The drone module is split as follows,
<div align="center">

||Description|Link|
|--|--|--|
| **Main-Pi** | The code base that will run on the main Raspberry Pi that handles data accusation from the individual sensors, packaging and sending of that data to the remote server. |[GitHub](https://github.com/lboroWMEME-TeamProject/Main-Pi) |
| **Geiger-Counter** | Code for Raspberry Pi Pico to get the sensor data from the Geiger counter  |[GitHub](https://github.com/lboroWMEME-TeamProject/Geiger-Counter) |
| **EnviroSensor** | Code to operate and control the Enviro+ Sensor with a Raspberry Pi |[GitHub](https://github.com/lboroWMEME-TeamProject/EnviroSensor) |
| **Ai-Cam** | Code to run the AI object detection on the raspberry Pi 4 and send its data to the Main Pi |[GitHub](https://github.com/lboroWMEME-TeamProject/ai-cam) |
| **Thermal-Cam** | Code to run and get images from the thermal camera |GitHub|


</div>