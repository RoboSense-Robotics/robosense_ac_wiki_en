# Tools  
## Collection  
Active Camera collection software package developed based on ros2, and through parameter configuration, it realizes the function of collecting data from different nodes. The data format collected supports .db3 and .mcap two formats according to different collection configurations.  
[Click to learn more](http://10.10.0.20/super_sensor_sdk/ros2_sdk/sdk_infra/-/blob/main/modules/ros2_collect/README_zh.md)  

## Monitoring  
Monitor some metrics of interest in ros2, such as: memory/CPU/IO usage, message frame rate, the difference between message timestamp and current system time, etc. The monitoring results will be output through logs and topics. At the same time, the software package also provides a python script to generate visual reports from the monitoring result data, which can locally generate html format reports containing simple statistical results and line charts.  
[Click to learn more](http://10.10.0.20/super_sensor_sdk/ros2_sdk/rs_monitor/-/blob/main/README_cn.md)  

## Calibration  

## Cross-compilation 
This tool is used to manage the cross-platform compilation and local compilation environment Docker container of Super Sensor SDK. It includes container management, image management, and automated environment setup functions.   
[Click to learn more](http://gitlab.robosense.cn/super_sensor_sdk/ros2_sdk/sdk_infra/-/blob/main/tools/cross_compilation/README_zh.md)  