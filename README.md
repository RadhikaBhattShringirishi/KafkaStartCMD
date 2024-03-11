# KafkaStartCMD
Installation of Kafka and zookeeper on windows 11(complete setup using cmd)::

1. zookeeper-server-start.bat ..\..\config\zookeeper.properties

2. kafka-server-start.bat ..\..\config\server.properties

3. kafka-topics.bat --create --topic my-topic --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3

4. kafka-console-producer.bat --broker-list localhost:9092 --topic my-topic

5. kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic my-topic --from-beginning
