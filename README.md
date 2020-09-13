# vagrant devbox

## Introduction

Simple vagrant Centos machine, with some useful stuff provisioned via ansible:

 - docker
 - java
 - jenkins
 - nodejs
 - apache

## Usage

To create and provision the machine:

`vagrant up`

To ssh in as vagrant user:

`vagrant ssh` and sudo as needed.

## Jenkins

Available at http://localhost:8080. Username "admin" password "pass1234".
Jenkins installs with blueocean & workflow-aggregator (pipeline) plugins, which bring in a load of dependent plugins.

## TODO

 - nexus
 - certbot
 - rancher
 - portainer
 - prometheus
 - grafana
 - portworx
 - spinnaker
