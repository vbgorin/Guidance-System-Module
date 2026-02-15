# Guidance_System_Module
Development and creation of an autonomous guidance system module with a laser designator for a CubeSat 1U spacecraft, which provides automatic two-axis guidance with a ±40° field of view, radio data reception and transmission, and is compatible with CubeSat standards in terms of dimensions, mounting, and vibration resistance.

The developed module is an autonomous guidance system with a laser target designator, designed for installation in a CubeSat 1U spacecraft. The module implements a full cycle of control of the laser beam direction in two mutually perpendicular planes with the ability to remotely control via a radio channel. The main functional capabilities include: 

1. Automatic two-axis guidance - the laser beam originates from the geometric center of the CubeSat; the system provides rotation along two axes (tilt and roll) with a viewing angle of ±40° along each axis and a positioning step of 10°. Guidance accuracy is checked on a target from a distance of 1 meter;
2. Device operation algorithm - after switching on, the module initializes, sets itself to the initial position (0°, 0°), enters the radio command standby mode, and upon receiving a control message, performs the specified scanning sequences (horizontal, vertical and two diagonal) sending data on the current angles every 3 seconds;
3. Radio communication and data exchange – using a radio module; transmitted messages contain a unique device identifier, current tilt and rotation angles, and operating mode status. The system response time does not exceed 2 seconds;
4. Design features – the module is designed as a stand-alone unit, compatible with CubeSat 1U; the vibration-resistant housing is made of 3D-printed plastic;
5. Hardware and software implementation – based on an Arduino controller, servo drives, a laser module, and a power supply. The software implements control algorithms and command processing.
