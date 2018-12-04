# OpenSource Security Tooling

*disclaimer*: The following information was put together to the best of my knowledge. Software might change or vanish and maybe not fit your purpose, please see it as a collection of ideas and nothing more. Also this list was never meant to be complete. 

### About me
I am working as a security Analyst / Consultant for a while now. part of my private craziness is to provide the same (cyber-) security standard I want to achieve for my clients also for my private life, but purely based on open source (mainly)

## Antivirus
### ClamAV

## Firewall
Linux/Unix based firewalls are pretty common and so we have many different flavors available, the border between firewall and IDPS is a pretty tiny gray line, as most of the products can utilise snort or suricata (at least \*sense does it pretty well)
* https://www.pfsense.org/
* https://opnsense.org/ (fork of pfsense)
* https://vyos.io/
* https://www.ipfire.org/

### IDS / IDPS
In this area two of the standard products are available. Snort is maybe the most famous, and due to the changes introduced with version 3.x it will stay that way for a bit longer.
* https://www.snort.org/
* https://suricata-ids.org/

### Fail2Ban
More in the Host based firewall area is Fail2Ban, actually you can configure a lot of services whereas SSH is the standard. After some login attempts or access attempts Fail2Ban will block you on the host firewall.
*https://www.fail2ban.org/

## WAF (Web Application Firewall)
### ModSecurity
You can add this mod to your webserver (Apache works best, Nginx is still a bit of work) and add some WAF capabilities to it. Please take a look at all the different sources available, especially the OWASP ones.
* https://www.modsecurity.org/

## Password Manager
### Keepass
Keepass comes in many flavors, even when I just search my local linux it shows 3 different variants. What all of them have in common is the .kdbx format for the password file, which is fair enough to make it exchangeable
* https://search.f-droid.org/?q=keepass&lang=en
* https://keepass.info/

## Monitoring
### Nagios / Icinga / Zabbix
The availability of systems should still be of concern to most of the people. And even if the purpose is on security only you might want to consider monitoring the connections and load of a system, as it can be valuable information during attacks.
* https://www.zabbix.com/
* https://www.nagios.org/
* https://icinga.com/

###  ELK Stack
curl --data-binary @filename http://example.com/
* https://www.elastic.co/elk-stack
* https://github.com/johestephan/Configurations/tree/master/Elasticsearch

## Threat Intelligence
## MISP 
The Malware Indicator Sharing Platform is a wide used tool when it comes to the sharing of IOCs and attack descriptions. It is fairly easy (or at least well documented) to setup.
* http://www.misp-project.org/

## Vulnerability Scanning
### ELK + nmap
nmap on its own is the standard scanning tool since forever and thanks to the community also for the years to come. I would recommend to try the combination of vulscan + nmap + ELK
* https://github.com/scipag/vulscan
* https://www.elastic.co/blog/using-nmap-logstash-to-gain-insight-into-your-network
* https://github.com/logstash-plugins/logstash-codec-nmap

