# The Band Infrastruture to Communication and Change Data Capture among OBDS and OBS

## 🚀 Goal

Provides an infrastructure that allows capturing of any change in the OBDS (e.g., insert, update, delete) and sending it to a queue, as presented in Figure.

![alt text](debezium-architecture.png "Debezium")

## ⚙️ Requirements

1. Docker Compose

## 🔧 Install

First, creates a .env file with the following contain:

```
DEBEZIUM_VERSION=2.0
COMPOSE_PROJECT_NAME = theband-cdc-infrastruture
```
The last, in a terminal execute the following commnad to start the infrastructure


```bash
docker-compose up
```

To check: [http://localhost:19000]

## 🛠️ Stack

1. [Apache Kafka](https://kafka.apache.org/)
2. [Debezium](debezium.io/) 
3. [PostgreSQL](https://www.postgresql.org/)
4. [Kafdrop] (https://github.com/obsidiandynamics/kafdrop)

## 📕 Literature

1. [Debezium GitHub Examples](https://github.com/debezium/debezium-examples/tree/main/tutorial)

2. [Introduction to Debezium](https://www.baeldung.com/debezium-intro)

3. [kafka Drop](https://medium.com/azure-na-pratica/apache-kafka-kafdrop-docker-compose-montando-rapidamente-um-ambiente-para-testes-606cc76aa66)
