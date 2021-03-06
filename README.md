# vagrant devbox

## Introduction

Simple vagrant Centos machine, with some useful stuff provisioned via ansible:

 - docker
 - java
 - jenkins
 - nodejs
 - apache
 - nexus
 - gitea

## Usage

To create and provision the machine:

`vagrant up`

To ssh in as vagrant user:

`vagrant ssh` and sudo as needed.

## Jenkins

Available at http://localhost:8080.  Username "admin" password "pass1234".
Jenkins installs with blueocean & workflow-aggregator (pipeline) plugins, which bring in a load of dependent plugins.

## Nexus

Available at http://localhost:8081. Username "admin" password "pass124".

## Gitea

Available at http://localhost:3000, git ssh at ssh://localhost:8222.
First user registered becomes the admin user.

## TODO

 - certbot
 - rancher
 - portainer
 - prometheus
 - grafana
 - portworx
 - spinnaker
