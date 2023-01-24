# kafka client linux cmd

## to install kafka client
```sh
yum install kafka
yum install java
```
## to list the topics of a kafka cluster
```
cd bin
./kafka-topics.sh --bootstrap-server <msk broker endpoints:9092> --list
```
