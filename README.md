# Capture Data Changes (CDC) with Kafka and Debezium

This is just an experimental project to implement debezium with kafka-connect to listen to any changes from MySQL tables.

## Prerequisite

- MySQL

- Kafka

- Kafka Connect

- Debezium

## Installation

## Scenario

1. Run docker container.
2. Create a connector using kafka-connect REST API, here is the [Postman Collection](https://documenter.getpostman.com/view/1259641/RWM8Trgy) of my postman collection for this experiment (this step will automaticly create some kafka topics).
3. Look at existing topic, ensure that we have all topic that we created.
4. Consume a created topic previously.
5. Make any data changes of a certain table.
6. Watch consumer, make sure that the changes is captured by debezium, and then produced by kafka-connect as a message.
