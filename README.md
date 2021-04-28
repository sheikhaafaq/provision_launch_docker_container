Role Name
=========

Provision_docker
Configure docker setup and launch a docker container using image httpd , also retrive IP address of container and upload a webpage..
Requirements

-----------

User should have docker and webserver knowledge..

Role Variables
--------------

varible "container_name" and "ports" specifies the name of docker container and Expose port of the container resp.

Dependencies
------------

At all no dependency here. 

Example Playbook
----------------

 Example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
  vars_prompt:
          - name: "ExposePort"
            prompt: "\nEnter the port to expose container to the public( like 8080 ) "
            private: no
          - name: "ContainerName"
            prompt: "\nEnter the name for container( like mycontainer ) "
            private: no
  gather_facts: no

  remote_user: root
  roles:


License
-------

BSD

Author Information
------------------

Name: Sheikh Aafaq Rashid 
Linked: https://www.linkedin.com/in/sheikh-aafaq-rashid-585803158/
github: sheikhaafaq
ansible-galaxy: sheikhaafaq18
Email: sheikhaafaq18@gmail.com

