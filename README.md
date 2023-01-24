# kafka client linux cmd

```sh
# to get access to an ec2 instance
chmod 400 xxx.pem
ssh -i "xxx.pem" ec2-user@Public IPv4 DNS

# to install kafka client
yum install kafka
yum install java

# to list the topics of a kafka cluster
cd bin
./kafka-topics.sh --bootstrap-server <msk broker endpoints:9092> --list

# to delete one topic of a kafka cluster
./kafka-topics.sh --bootstrap-server <msk broker endpoints:9092> --delete --topic <topic name>

# to consume messages of a topic
./kafka-console-consumer.sh --bootstrap-server <msk broker endpoints:9092> --topic <topic name> (opt. from beginning)

# to create a topic
./kafka-topics.sh --bootstrap-server <msk broker endpoints:9092> --create --topic <topic name> --partitions 3 --replication-factor 2

# to produce messages into a topic of a kafka cluster
./kafka-console-producer.sh --broker-list <msk broker endpoints:9092> --topic <topic name>



```

