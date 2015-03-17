# Mesos pseudo cluster with connection to pseudo Hadoop cluster

If you need Mesos cluster with Chronos scheduler and your Mesos Slaves are talking to Cloudera Hadoop (CDH) you can use this fig (docker-compose) configuration to startup all neccessary services.

NOTE: CDH is not running within mesos but is just available from Mesos slave. 

###Requirements
* Virtualbox (brew cask install virtualbox)
* Docker (brew install boot2docker)
* Fig (brew install docker-compose)

###Intalled services
* Zookeeper
* Cloudera Hadoop
* Mesos
* Chronos

Start

    fig up -d

Stop

    fig stop

Mesos UI ```http://localhost:5050```
Chronos UI ```http://locahost:8081```
Resource manager UI ```http://localhost:8088```
Hdfs UI ```http://localhost:50070```
