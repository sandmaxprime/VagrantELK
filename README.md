# VagranELK

[![Twitter](https://img.shields.io/twitter/follow/sandmaxprime.svg?style=social)](https://twitter.com/sandmaxprime)
![Reddit User Karma](https://img.shields.io/reddit/user-karma/combined/sandmaxprime?style=social)
![YouTube Channel Views](https://img.shields.io/youtube/channel/views/UCUczlwCDjCLb0zBiTlQ4Mtw?style=social)
![Keybase BTC](https://img.shields.io/keybase/btc/sandmaxprime)
![Keybase ZEC](https://img.shields.io/keybase/zec/sandmaxprime)

---
## Vagrant Setup

Make sure your system has [VirtualBox](https://www.virtualbox.org/) installed. After this, download and install [Vagrant](https://www.vagrantup.com/downloads.html) for your system

---

## VM Config
The Vagrantfile will create a VirtualBox VM with the following configuration
```
RAM = 4096 MB
CPUs = 2
```
The VM is based on Ubuntu Bionic (18.04.LTS) and has the following installed:
* Elasticsearch 7.13
* Kibana 7.13
* OpenJDK 8

Kibana - http://localhost:5601
ElasticSearch - http://localhost:9200

---
## VM Creation

* Clone the repository
  
* Using terminal, navigate to the repository folder containing the VagrantFile and then ```vagrant up```

* This will then download the box file - This will take some time
* Post the download, the VM will be created and the provisioning will begin to install the packages.

---
