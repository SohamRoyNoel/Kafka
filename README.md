
# Kafka
# Starting Kafka
  - Start Zookeeper
  ```
  PS D:\Kafka\kafka_2.12-2.5.0> zookeeper-server-start.bat config\zookeeper.properties
  ```
  - Start Kafka
  ```
  PS D:\Kafka\kafka_2.12-2.5.0> kafka-server-start.bat config\server.properties
  ```
  ## Kafka Commands
  #### Topics
Kafka Topic Version: ***kafka-topics --version***; my version is: ***2.5.0 (Commit:66563e712b0b9f84)***
Get All Kafka Options: ***PS D:\Kafka\kafka_2.12-2.5.0> kafka-topics***
Create A Kafka Topic: ***kafka-topics --zookeeper 127.0.0.1:2181 --topic First_Topic --create --partitions 3 --replication-factor 1***
***[Remember: replication factor can not ever be greater then the brokers; that means if you start 1 kafka on a cluster, --replication-factor 1 should be >=1]***
    
