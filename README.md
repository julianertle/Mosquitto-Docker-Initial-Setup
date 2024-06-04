MQTT Broker with Eclipse Mosquitto

This repository contains a Docker Compose configuration to run an MQTT broker using Eclipse Mosquitto.
Getting Started

To get started with this MQTT broker, follow these steps:
Prerequisites

Before you begin, make sure you have Docker and Docker Compose installed on your system.

    Docker installation guide: Install Docker
    Docker Compose installation guide: Install Docker Compose

Usage

    Clone this repository to your local machine:

    bash

git clone [<repository-url>](https://github.com/julianertle/Mosquitto-Docker-Initial-Setup.git)

Navigate to the repository directory:


cd <repository-directory>

Start the MQTT broker using Docker Compose:

bash

    docker-compose up -d

    This command will start the MQTT broker container in detached mode, allowing it to run in the background.

    You can now connect to the MQTT broker using the specified port (default is 1883) from your MQTT clients.

Configuration Options

    Anonymous Access: By default, anonymous access is allowed. You can modify this behavior in the mosquitto.conf file.

    Persistence: Persistence information on client subscriptions and retained messages is enabled by default. You can modify the persistence settings in the mosquitto.conf file.

Accessing Logs and Data

    Logs: Log files are stored in the log directory.

    Data: Persistent data, including the MQTT database (mosquitto.db), is stored in the data directory.

Contributing

Contributions are welcome! If you have suggestions, feature requests, or find any issues, please open an issue or create a pull request.
