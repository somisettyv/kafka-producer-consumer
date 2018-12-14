# kafka-producer-consumer


Important Kafka Propeties 

    Find the Kakfa Broker details from the VM where you install the Kakfa 
    
    props.put(ConsumerConfig.BOOTSTRAP_SERVERS_CONFIG, IKafkaConstants.KAFKA_BROKERS);

    public static String KAFKA_BROKERS = "172.18.0.2:6667";

How to find the Broker from VM where you install the Kakfa


Deploy the Jar 

Run the Jar 


Run the Kakfa Consumbers directly on the Kakfa VM

Create a Kakfa Topci as follows 

    ./bin/kafka-topics.sh --create --zookeeper c38-node1.example-labs.com:2181 --replication-factor 1 --partitions 1 --topic demo
    

Produce The message 

    ./bin/kafka-console-producer.sh --broker-list 172.18.0.2:6667 --topic demo

Consume the Message 
 
     /usr/hdp/current/kafka-broker/bin/kafka-console-consumer.sh --zookeeper localhost:2181 --topic demo --from-beginning
