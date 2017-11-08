# JHLidarLite_V3_TX2

Modified to work on the Jetson TX2 with the new (GARMIN) Lidar Lite V3

Interface for PulsedLight, Inc Lidar-Lite V3 Garmin to NVIDIA Jetson TX2 Development Kit over I2C.

http://pulsedlight3d.com

Note: For interfacing LidarLite V1 to Jetson TK1, see https://github.com/jetsonhacks/JHLidarLite

Requires:

$ sudo apt-get install libi2c-dev i2c-tools

The Lidar-Lite appears as 0x62 on i2c bus 1 on the Jetson TK1 with this wiring:

<blockquote><p>VCC J3A1-1 ->  
Lidar-Lite (+)    
5V (red wire)<br>
GND J3A1-14 ->  Lidar-Lite (-)<br>
SCL J3A1-18 ->  Lidar-Lite (SCL)<br>
SDA J3A1-20 ->  Lidar-Lite (SDA)</p></blockquote>

//Not sure if true on high current 5v supplies... - mrgibbes
Lidar-Lite V2 requires a 680uF capacitor between 5V and GND. See documentation for wiring.
