
# Kafka Sample Project

>This repository demonstrates a simple Kafka setup using Docker, with separate NestJS-based producer and consumer services.

## Table of Contents
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Kafka UI Dashboard](#kafka-ui-dashboard)
- [Running the Producer](#running-the-producer)
- [Running the Consumer](#running-the-consumer)

## Overview
This project provides:
- A local Kafka broker and UI dashboard via Docker Compose
- A NestJS producer service (`producer/`) to send messages to Kafka
- A NestJS consumer service (`consumer/`) to receive messages from Kafka

## Prerequisites
- [Docker](https://www.docker.com/get-started)
- [Node.js](https://nodejs.org/) & [Yarn](https://yarnpkg.com/) (for running producer/consumer)

## Setup
Start Kafka and the UI dashboard:

```bash
docker compose up -d
```

## Kafka UI Dashboard
Once started, access the Kafka UI dashboard at [http://localhost:8080](http://localhost:8080).

## Running the Producer
1. Navigate to the `producer` folder:
   ```bash
   cd producer
   yarn install
   yarn start
   ```
2. The producer will send messages to the Kafka broker.

## Running the Consumer
1. Navigate to the `consumer` folder:
   ```bash
   cd consumer
   yarn install
   yarn start
   ```
2. The consumer will listen for messages from the Kafka broker.

## License
This project is licensed under the MIT License.
