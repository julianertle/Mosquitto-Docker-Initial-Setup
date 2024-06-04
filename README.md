
# README

### MQTT Broker with Eclipse Mosquitto

This repository contains a Docker Compose configuration to run an MQTT broker using Eclipse Mosquitto on your **local machine**.

**Getting Started:**

Before you begin, make sure you have Docker and Docker Compose installed on your system.

    Install Docker
    Install Docker Compose

**Usage**

    Clone this repository to your local machine, you can use Visual Studio Code for that:
    
    git clone https://github.com/julianertle/Mosquitto-Docker-Initial-Setup.git


Navigate to the repository directory:

    cd <repository-directory>
Start your docker instance.
Now start the MQTT broker in a terminal using Docker Compose:

    docker-compose up -d

You can now connect to the MQTT broker using the specified port (default is 1883) from your MQTT clients.

Open another terminal and subscribe to your broker:

    docker-compose exec mosquitto mosquitto_sub -h localhost -p 1883 -t test/topic

Open one more terminal and publish a message to the broker: 

    docker-compose exec mosquitto mosquitto_pub -h localhost -p 1883 -t test/topic -m "Hello World" 


