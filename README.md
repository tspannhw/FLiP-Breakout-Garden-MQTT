# FLiP-Breakout-Garden-MQTT
mqtt, sensors, raspberry pi 3, pimoroni breakout garden, apache pulsar, python



## Build Pulsar/MQTT Topic

bin/pulsar-admin topics create persistent://public/default/breakout

bin/pulsar-client consume "persistent://public/default/breakout" -s "brkoutr" -n 0

