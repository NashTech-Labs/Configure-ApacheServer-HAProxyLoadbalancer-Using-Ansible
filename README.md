## Ansible Roles

Ansible roles are used to simplify Ansible playbook which means we can break a complex Ansible playbook in independent and reusable roles that are used to automatically load certain var_files, tasks, and handlers as per pre-defined file structure

## HA Proxy
HAProxy is a free,  fast and reliable solution offering high availability, load balancing, and proxying for TCP and HTTP-based applications.

In this project we are creating an ansible role myapache to configure Httpd WebServer and another ansible role myloadbalancer to configure HAProxy LB.
We need to combine both of these roles controlling webserver versions and solving challenge for host ip’s addition dynamically over each Managed Node in HAProxy.cfg file.

============================================================================

Before using this project you need to set up your playbook file to call the roles and also setup your hosts. and then run the playbook.
We successfully completed the task and we can verify it by running the web page.
We can notice the IP is switching even though the IP address which we are using at browser is same. This proves that the HAproxy is working fine.
