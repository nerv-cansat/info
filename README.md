# NERV Team CanSat 2021/2022

## Our team
**Aleksander Ałaszewski** - Team leader, mechanical design.  
**Jakub Sztuka** - Electrical design, software design, GitHub maintainer. [GitHub page](https://github.com/sztvka/)  
**Dawid Frukacz** - Ground support equipment and recovery system.  
**Jan Pawelec** - Outreach and graphic design. Instagram maintainer.  
**Paweł Kelm** - Supervisor of the project. Professor at Lodz University of Technology.

## General Architecture
Our CanSat was built out of a handmade carbon fiber tube, with a 3D-printed interior. All of the electronics were based around the CanSatKit PCB featuring ATSAMD21G18 MCU (Arduino M0), LoRa wireless communication module and a microSD card slot. Everything was powered from a 2S LiPo. The design used a ripstop nylon parachute as the primary means to control descent rate. The parachute was backed up via a BLDC motor as a mean to slow down right before impact.

## Mission objectives
The project had three objectives:  
- Collecting and analyzing air quality data at different altitudes
- Testing the viability of low-light solar cells for powering basic subsystems (onboard real-time clock)
- Testing the viability of propeller braking in addition to a parachute

### Collecting air quality data
The CanSat was equipped with:
- DS18B20 temperature sensor
- BMP280 pressure sensor
- AHT20 Humidity Sensor
- Honeywell CRIR-E1 CO2 sensor
- Sensirion SPS-30 particulate matter sensor
- MICS-5524 gas sensor
- MinIMU-9 v5 accelerometer & gyroscope combo   
  
This sensor array allowed to pinpoint altitude and falling speed, as well as air pollution at different levels.

### Energy harvesting
The CanSat was equipped with:
- DS3231 Real-Time-Clock module
- AM-1085CA Solar panel with 2 supercapacitors
  
These components allowed for precise timekeeping

### Propeller Braking
The CanSat was equipped with:
- VL53L1X ToF infrared distance sensor
- T-Motor F1103 8000KV BLDC motor with a HQprop T2x2.5x3 2” propeller
- HGLRC BS28A ESC
  
These components allowed for approximating distance to the ground and slowing down the satellite right before impact.

## Mission Execution
Our satellite was dropped from 1500 meters high on the Błędowska desert via a PTR SOLARIS rocket. The satellite sucessfully transmitted data over LoRa radio. Every subsystem was working perfectly, except the parachute, that flew away due to bad mounting. Despite the descent speed of over 150km/h (measured terminal velocity with no parachute) our CanSat captured vital atmospheric data and survived the impact with every subsystem functioning, except the ground distance sensor. We were able to tell how high the ongoing sandstorm spanned and measure air pollution high up in the air.


## Gallery


![](https://github.com/nerv-cansat/info/blob/main/img/IMG_0322.JPG?raw=true)
![](https://github.com/nerv-cansat/info/blob/main/img/IMG_0332.JPG?raw=true)
![](https://github.com/nerv-cansat/info/blob/main/img/IMG_0334.JPG?raw=true)
