## Kafka Offset Monitor Dockerfile


This repository contains **Dockerfile** of [Kafka Offset Monitor](https://github.com/quantifind/KafkaOffsetMonitor) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/hwestphal/kafka-offset-monitor/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [dockerfile/java:oracle-java7](http://dockerfile.github.io/#/java)


### Usage

Create a data directory on your host and put there a `.conf` file with your favorite [command line options](https://github.com/quantifind/KafkaOffsetMonitor#running-it), then:

    docker run -d -p 8080:8080 -v <persistent-data-dir>:/data hwestphal/kafka-offset-monitor

After few seconds, open `http://<host>:8080/` to see the starting page.
