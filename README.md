install mongoDB
install pymongo

Install Kafka : https://hevodata.com/blog/how-to-install-kafka-on-ubuntu/ https://kafka.apache.org/quickstart
kafka user: olawale

\*\* create topic to store events

```
bin/kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092
```

\*\* show details such as the partition count

```
bin/kafka-topics.sh --describe --topic quickstart-events --bootstrap-server localhost:9092
```

\*\* write some events into the topic

```
bin/kafka-console-producer.sh --topic quickstart-events --bootstrap-server localhost:9092
```

\*\* read the events

```
bin/kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092
```
