# confluent-kafka-basic

How to run the example

1. Run the zookeeper
        ./bin/zookeeper-server-start ./etc/kafka/zookeeper.properties
        
2. Run kafka
        ./bin/kafka-server-start ./etc/kafka/server.properties
        
3. Run the spring boot app
        ./gradlew bootRun
        
4. Test with below curl command
        curl -X POST -F 'message=test' http://localhost:9000/kafka/publish                                



# Zookeeper is used for maintaining a centralized configuration information, naming, providing distributed synchronization, and providing group services. Very notably softwares likes solr uses zookeeper to maintain its configurations across the cluster. APache kafka also uses zookeeper to manage configuration.