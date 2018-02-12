Role Name
=========

 Ansible role to install node_exporter in centos 7 and add it as a service

Requirements
------------
The client node should have access to download the packages from the repos.


Role Variables
--------------

vars/main.yml
 node_exporter_download_location 
 node_exporter_download_url
 node_exporter_downlaod_file : name of the tar file being downloaded by 'node_exporter_download_url'

templates
   templates/node_exporter.init.j2 - init file for centos 6

Dependencies
------------
N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:


	- name: starting the node_exporter script
	  hosts: host1
	  tasks:
	  - include_role:
	       name: ansible-role-node_exporter_prometheus

License
-------

Apache

Author Information
------------------

- ebin

