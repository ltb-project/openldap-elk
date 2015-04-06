# OpenLDAP ELK
ELK configuration to parse OpenLDAP logs

## Presentation

ELK (ElasticSearch/Logstash/Kibana) is a suite of tools that allow to parse, store and display data from logs. This project provides some sample configurations of these tools in order to get statistics from OpenLDAP logs.

## Usage

### Logstash

Use the files in logstash as configurations. For example, copy them in /etc/logstash/conf.d and run:
    /opt/logstash/bin/logstash agent -f /etc/logstash/conf.d/


