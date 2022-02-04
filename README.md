# FLiP-Breakout-Garden-MQTT
mqtt, sensors, raspberry pi 3, pimoroni breakout garden, apache pulsar, python



## Build Pulsar/MQTT Topic

bin/pulsar-admin topics create persistent://public/default/breakout

bin/pulsar-client consume "persistent://public/default/breakout" -s "brkoutr" -n 0

## Example Data

````
----- got message -----
key:[null], properties:[], content:{"systemtime": "02/04/2022 14:19:58", "bme680_pressure": "1007.57", "bme680_tempf": "74.84", "BH1745_blue": "9.0", "lsm303d_magnetometer": "-00.03 : +00.25 : +00.14", "BH1745_red": "28.6", "diskusage": "10468.9", "end": "1644002398.1865404", "ltr559_prox": "0000", "cputemp": 39, "te": "403.8052625656128", "bme680_humidity": "44.687", "ltr559_lux": "020.18", "ipaddress": "192.168.1.229", "host": "piups", "imgnamep": "/opt/demo/images/bog_image_p_20220204191958_d79c8958-fc8a-4774-8412-4ac6e6bec48a.jpg", "memory": 20.4, "BH1745_clear": "20.0", "VL53L1X_distance_in_mm": 317, "uuid": "20220204191958_d79c8958-fc8a-4774-8412-4ac6e6bec48a", "imgname": "/opt/demo/images/bog_image_20220204191958_d79c8958-fc8a-4774-8412-4ac6e6bec48a.jpg", "lsm303d_accelerometer": "-00.01g : -01.00g : -00.05g", "bme680_tempc": "23.80", "BH1745_green": "21.0", "starttime": "02/04/2022 14:13:14"}

````
