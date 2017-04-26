
# A Docker Image for Cloudera Quickstart

Run the CDH Quick Start image in a docker container.


## Install

This image is somewhat large, so you might want to do a separate

    docker pull anuk87/cdh-spark

to install.


## Use

Spin it up with

    docker run -td anuk87/cdh-spark

get the container id from

    docker ps

watch logs with

    docker logs -f <container_id>

attach to the container with

    docker exec -it <container_id> bash -l

then run any of the usual cdh commands

    hadoop fs -ls /
    spark-submit
    hive
etc.


## Components

- Apache Hadoop (Common, HDFS, MapReduce, YARN)
- Apache Hive
- Hue (Apache licensed)
- Apache Spark


## Links

Pull the image on Docker Hub:

Github page:

[Cloudera Documentation](http://www.cloudera.com/content/cloudera/en/documentation/core/latest/)


## Credits

This image is a modified fork of
[silicon-valley-data-science/docker-cdh](https://github.com/silicon-valley-data-science/docker-cdh)
