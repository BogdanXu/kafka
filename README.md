# kafka
Kafka practice to produce/read messages with the use of recent wikipedia changes from https://stream.wikimedia.org/v2/stream/recentchange

How to run: 

Open 4 wsl terminals 

Navigate to where kafka is installed locally for 1st and 2nd terminal 

1st terminal: Start zookeeper with bin/zookeeper-server-start.sh config/zookeeper.properties 

2nd terminal: Start kafka server (brokers) with bin/kafka-server-start.sh config/server.properties 

3rd terminal: navigate to producer app (kafka-wikimedia-producer), run with mvn spring-boot:run, see that wikimedia messages are produced 

4th terminal: navigate to consumer app (kafka-consumer), run to see that the messages are consumed 
