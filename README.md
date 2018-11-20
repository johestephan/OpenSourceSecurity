# OpenSource Security Tooling

*disclaimer*: The following information was put together to the best of my knowledge. Software might change or vanish and maybe not fit your purpose, please see it as a collection of ideas and nothing more.

### About me
I am working as a security Analyst / Consultant for a while now. part of my private craziness is to provide the same (cyber-) security standard I want to achieve for my clients also for my private life, but purely based on open source (mainly)

## Antivirus
### ClamAV

## Firewall

## Password Manager
### Keepass

## Monitoring
### Nagios / Icinga / Zabbix
The availability of systems should still be of concern to most of the people. And even if the purpose is on security only you might want to consider monitoring the connections and load of a system, as it can be valuable information during attacks.
* https://www.zabbix.com/
* https://www.nagios.org/
* https://icinga.com/
###  ELK Stack
While enterprise user turn to SIEM solutions in order to detect and protect, the ELK Stack (Elasticsearch + Logstash + Kibana) provides a solid approach. I for myself use it to collect the logs of my cloud servers and check for "interesting" log entries.
* https://www.elastic.co/elk-stack
* https://github.com/johestephan/Configurations/tree/master/Elasticsearch
