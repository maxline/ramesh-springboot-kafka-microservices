# Spring boot apache kafka Udemy course by Ramesh 

https://udemy.com/course/spring-boot-and-apache-kafka

Source code
https://github.com/RameshMF/springboot-kafka-course


## Run Kafka Server
```
$ cd kafka
$ kafka % KAFKA_CLUSTER_ID="$(bin/kafka-storage.sh random-uuid)"                                   
$ kafka % bin/kafka-storage.sh format --standalone -t $KAFKA_CLUSTER_ID -c config/server.properties
$ kafka % bin/kafka-server-start.sh config/server.properties
```

## Usage scenarios
POST
http://localhost:8080/api/v1/order
```
{
  "orderId": "111",
  "name": "first order",
  "qty": 7
}
```