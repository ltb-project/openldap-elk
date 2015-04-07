# OpenLDAP ELK
ELK configuration to parse OpenLDAP logs

## Presentation

ELK (ElasticSearch/Logstash/Kibana) is a suite of tools that allow to parse, store and display data from logs. This project provides some sample configurations of these tools in order to get statistics from OpenLDAP logs.

## Usage

### Logstash

Use the files in logstash as configurations. For example, copy them in /etc/logstash/conf.d and run:
    /opt/logstash/bin/logstash agent -f /etc/logstash/conf.d/

### Elastic Search

You just need to have Elastic Search running on the default port

### Kibana 3

In Kibana 3, select Load > Advanced > Local File and import dashbords. For now, this project provides 2 dashboards:
* OpenLDAP operations : statistics on LDAP operations (Bind, Add, Search, ...)
* LDAP error codes : statistics on error codes (No such object, Invalid credentials, ...)

