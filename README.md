# NSM
Network Security Monitoring
Installing Virtualbox
Install Virutalbox from https://www.virtualbox.org/wiki/Downloads
Download Ubuntu 20.04 from https://releases.ubuntu.com/20.04/
Setup the Ubuntu instance and add 2 adapters to the Virtual Machine
![image](https://user-images.githubusercontent.com/30376802/176098974-e4eff834-57d5-47dd-a255-67a9c727bc6f.png)
You can keep both adapters on NAT or Bridge
Install net-tools
apt-get install net-tools
Setup Promiscuous mode
ifconfig adpter-name <eth0> promisc
Install Suricata
apt-get update && apt-get install suricata
Install Zeek
  git clone --recursive https://github.com/zeek/zeek
  ./configure && make && sudo make install
refer - https://github.com/zeek/zeek
Install ElasticSearch
Installation of ElasticSearch varies depending on which version you install, I used 7.x so will attach link to that, since I used Debian as my bas OS but ElasticSearch can be installed on other platform too
  https://www.elastic.co/guide/en/elasticsearch/reference/7.17/install-elasticsearch.html
Install Kibana
Installting Kibana will follow similar process as ElasticSearch
  https://www.elastic.co/guide/en/kibana/7.17/install.html
Installing FileBeat
Similarly with FileBeat too
  https://www.elastic.co/guide/en/beats/filebeat/7.17/filebeat-installation-configuration.html
I'd suggest reading all configurations to understand its capabilities and scalability.
My Configuration files are available in config directory

