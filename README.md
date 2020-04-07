# Web Server Provisioning Workflow Lab
## Introduction
One of the benefits of Ansible and the Ansible Automation Platform is its ability to automate across departments in your IT oranziation.  For instace, let's say a new webserver is required. In the past, the server team would be notifed and would begin provisioning the new server.  The network team would also be notified to begin its process of configuring switchports, opening firewall rules, or setting up a load balancer.   With Ansible Tower, we can coordinate these efforts into a single workflow.  This lab will demonstrate such a workflow by confiuging a switch port, performing an update on a CentOS server, installing a new admin user, installing NGINX, and finally emailing a report.  Playbooks are provided to configure Tower for the lab.  

![Tower Workflow](docs/workflow1.png)


## Requirements

This lab was tested using Ansbile 2.9 and Tower 3.6.  It assumes you have the following

- Ansible Tower 
- [Tower CLI](https://docs.ansible.com/ansible-tower/3.5.3/html/towerapi/tower_cli.html) installed on your Tower server
- Centos 7 VM to similute our web server
- [Arista vEOS VM](https://www.arista.com/en/support/software-download) with at least three NICs to simulate our switch.  A sample config is provided in the docs folder.
- Optional:  A gmail email address to send the report.


## Installation

1. In order to configure Tower, we will use the *tower_lab_provision.yml* playbook.   SSH into Tower and clone this repo.

```
git clone https://github.com/gejames/Linux-Webserver-Tower-Lab.git
```

2. Edit the default variables in tower/vars/webdemo_tower.yml for your environment.  

3. Run the playbook tower_lab_provision.yml on the Tower server.  It will ask for your Tower credentials. 

```
ansible-playbook tower_lab_provision.yml
```

## Launching the Workflow


## Reseting the lab










