# Tomcat 7 Infrastructure provisioning using Ansible Automation

Ansible 2.7

* Gathers Ansible facts 
* Downloads and set EPEL repository , Add firewall rules for Tomcat as per OS type
* Installs dependency packages
* Performs environmental  pre and post-checks
* Installs  Java 1.7
* Adds System User and group for Tomcat
* Use of Notifiers for service handlers
* Downloads, Extracts and Symlinks Tomcat directory
* Changes ownership, Configure tomcat parameters and starts the service
* Deploys a Calendar war package to WEBAPPS of tomcat and re-initiates the service

## Steps
```
git clone https://github.com/pranav-sharma429/Tomcat-spin.git
```

```
cd Tomcat-spin
```

```
ansible-playbook -i hosts site.yml
```
