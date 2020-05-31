# DNS Server

## Table of contents
 * [General info](#general-info)
 * [Techonologies](#technologies)
 * [Setup](#setup)

## General info
Project contain examples of configuration files, include mail configuration for containerized DNS server on ARM architecture machines. It is perfect for Raspbery Pi.

## Technologies
 * Bind9
 * docker-compose

## Setup
> docker-compose

### How add new domain?
In *./named.conf.local* file add new zone for new domain. We create it based on provided examples <br />
In *./named/* directory add new configuration file. It can be created based on provided examples. Files names must end with *.conf* <br />
You can check if configurations are valid by *docker exec dns named-checkconf /etc/bind/named.conf* command <br />
Don't forget to restart container *docker restart dns* <br />



