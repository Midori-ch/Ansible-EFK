# Ansible-EFK
Ansible playbook for EFK deploy.(elasticsearch + fluentd + kibana)

# Items
## Install on server node (Elasticsearch + Kibana)
* jdk 8
* [elasticsearch 7.3](https://www.elastic.co/guide/en/elasticsearch/reference/current/rpm.html)
* [kibana 7.3](https://www.elastic.co/guide/en/kibana/current/rpm.html)
* httpd
## Installe on Fluent(td-agent) node
* [kernel and limits settings.](https://docs.fluentd.org/installation/before-install                                                                                          )
* td-agent
* td-agent-plugins
* syslog

# Prerequisite
* Correction time
* CentOS 7 up
* Direct ssh
* Ansible 2.8

# Steps
## Change inventory file 
[server]  
192.168.1.20  

[tgagents]
192.168.1.21
## Run the Playbook
`$ ansible-playbook -i inventory site.yml`
