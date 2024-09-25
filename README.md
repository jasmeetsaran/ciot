# IoT Workshop - 2024 - Carrier
==============================================

## World before IoT (Internet of Things)
M2M or Machine to Machine enables communication between two machines performing smaller piece of a common task.

### Examples:
- Electrical telegraph and fax
- Caller ID Technology
- Industrial Machines & Production Lines

## IoT in Simple Words
IoT is simply making all the physical devices/things connect to the internet and let them exchange information.

> Where thing is any device that can give information or act upon given signal or information.

## The Goal of an IoT System

**Gather, Send, Receive & Act on the Information**

## IoT Lifecycle
Sense > Connect > Collect > Infer > Act

## Real world applications discussed:
 - Health Care
 - Smart Cities
 - Smart Home
 - Connected Vehicles

## IoT Architecture Discussion
 - ESP32 (Device) to Raspberry Pi (Device)
 - Esp32 (Device) to AWS (Cloud)


# IoT Protocols

- Constrained Devices vs Regular Devices
- Need for IoT Protocols

Popular protocols
- HTTP & WebSockets
- MQTT

### HTTP Challenges
- Verbose and Text heavy
- One Way communication

### HTTP Workarounds
- Long or frequent polling or both

### WebSockets
- Can create a long and persistant connection.
- Can send data back and forth anytime during Session

### MQTT
- Simple Messaging Protocol
- Works on top of TCP
- Publish / Subscribe Architecture
- Binary protocol
- Minimal Overhead
- Designed for unreliable networks
- Data agnostic

### MQTT Topics and Wildcards
- (+) Single level - home/groundFloor/+/temperature
- (#) Multi level -  office/level1/#

## MQTT Sparkplug Specification discussion
https://sparkplug.eclipse.org/specification/version/2.2/documents/sparkplug-specification-2.2.pdf

# LABS

### Setting up Raspberry Pi
https://projects.raspberrypi.org/en/projects/raspberry-pi-setting-up/2

SSH command for login: **ssh username@ip address**

### Getting Started with Arduino IDE
https://docs.arduino.cc/software/ide-v2/tutorials/getting-started-ide-v2/

### Connect DHT22 with ESP32 and send data to ThingSpeak
https://github.com/jasmeetsaran/ciot/blob/main/esp-dht-thingspeak

Use https://thingspeak.com/ to visualize your data in the form of graphs and charts.

### Setup Mosquitto Broker on Raspberry Pi
https://github.com/jasmeetsaran/ciot/blob/main/setup-mosquitto-pi.md

### Setup Node Red on Raspberry Pi
https://nodered.org/docs/getting-started/raspberrypi

### Node Red Flow (MQTT Dashboard)
https://github.com/jasmeetsaran/ciot/blob/main/nodered-mqtt-dashboard-flow

### Send DHT22 Sensor data via ESP32 to Raspberry Pi (Node Red Dashboard over MQTT)
https://github.com/jasmeetsaran/ciot/blob/main/dht-mqtt-json 

### Node Red Flow (HTTP to MQTT)
https://github.com/jasmeetsaran/ciot/blob/main/http-to-mqtt

### Getting Started with AWS IoT Core
https://docs.aws.amazon.com/iot/latest/developerguide/iot-gs.html

### Send Data to AWS IoT Core device
https://github.com/jasmeetsaran/ciot/tree/main/basic-pubsub

### Send DHT22 Sensor data via ESP32 to AWS IoT Core
https://github.com/jasmeetsaran/ciot/blob/main/dht22-aws-mqtt

### Getting Started with GreenGrass
https://docs.aws.amazon.com/greengrass/v2/developerguide/what-is-iot-greengrass.html

https://awscli.amazonaws.com/v2/documentation/api/latest/reference/greengrassv2/index.html

## Setup GreenGrass with on Pi along with custom component creation
https://github.com/jasmeetsaran/ciot/blob/main/gg-commands.md
