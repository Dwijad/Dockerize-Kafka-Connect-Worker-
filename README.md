# Dockerize Confluent Kafka Connect Worker

Build docker image for secured confluent kafka Connect worker in your local docker environment with Debzeium MySQL connector and JDBC source/sink connector. Subsequently deploy the kafka connect worker in kubernetes cluster in a distributed way. 

The image is available directly from [Docker Hub](https://hub.docker.com/r/wurstmeister/kafka/)
### Prerequisite
 - You have a local kafka cluster running in any of the PLAINTEXT, SSL, SASL_PLAINTEXT, SASL_SSL mode.
 -  You have a schema registry server running with/without SSL mode.
 -  You want to convert data for Kafka Connect to and from in Avro format.
 -  For testing query based CDC connector a MySQL DB server is configured and running.
 -  For rebuilding Docker image, install docker with buildx plugin as described [here](https://docs.docker.com/engine/install/ubuntu/).

### Usage
#### Use case - 1
Run Kafka connect worker with Kafka broker listener configured in PLAINTEXT mode. The schema registry is running in either secured or non-secured mode.



https://github.com/1ambda/docker-kafka-connect
https://github.com/SAP/kafka-connect-sap
https://github.com/debezium/debezium
https://github.com/wurstmeister/kafka-docker
https://joelforjava.com/blog/2019/10/27/adding-ssl-encryption-to-kafka-connector.html 
<!--stackedit_data:
eyJoaXN0b3J5IjpbOTI5MDYzNjE5LDk5MTExMzE2NCwyMDE0MT
IzNzY1LC04Nzg3NzEwMTcsLTQ4MjQyOTY0Nyw3MTkyMDUyNjBd
fQ==
-->