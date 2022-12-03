# microservices-demo
Event driven microservice powered by kafka

Submodule introductions:
- twitter-to-kafka-service : A Mock app to return random strings
- kafka : contains the configs and interfaces and impl for the kafka related modules
  - Kafka-admin : programmatically adds the Topic to the schema registry
  - kafka-producer : producer interfaces and impl
  - kafka-model : auto generated from the avro schema (in resources folder)
  - kafka-consumer : contains the configs for the kafka consumer
- app-config-data : Contains the config data needed for the applications
- common-config : contains the retry logic
- docker-compose : contains the docker compose scripts needed to deploy the app and infra i.e kafka clusters

# Build instructions: 

mvn clean install -DskipTests

(The tests are not yet in place)



