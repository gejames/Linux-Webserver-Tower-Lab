# Web Server Provisioning Workflow Lab
## Introduction
One of the benefits of the Ansible and the Ansible Automation Platform is its ability to automate across departments in your IT oranziation.  For instace, let's say a new webserver is required. In the past, the server team would be notifed and would begin provisioning the new server.  The network team would also be notified begin its process to configure switchports, open firewall rules, or setup load balancers.   With Ansible Tower, we can coordinate these efforts into a single workflow.  This lab will demonstrate such a workflow by confiuging a switch port, performing an update on a CentOS server, installing a new admin user, installing NGINX, and finally emailing a report.  We will use Ansible Tower to create a powerful workflow.   Playbooks are provided to configure Tower for the lab.

## Requirements

The lab assumes you have the following

- Ansible Tower
- Centos 7 VM to similute our web server
- Arista vEOS VM with at least three NICs to simulate our switch
- Optional:  A gmail email address to send the report.











