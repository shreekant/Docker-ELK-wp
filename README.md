# Requirements
Imagine you’re part of a team that is starting a blogging application that would eventually run on the cloud (let’s assume it's AWS). 
The team has decided to use Wordpress to get a simple blog running as a start. 
Your team of developers wants you to help them monitor their application and the computers their application are running on. 
Since cloud is the target infrastructure, you decide to use centralised logging and dashboarding using the ELK (ElasticSearch, Logstash, Kibana) stack. The entire infrastructure is intended to be a container based system.

# What to do?
To achieve the above, you would need to:
  1. Create a Docker compose based ELK setup, so that it's repeatable and demonstrable on a development machine.
  2. Use Ansible for provisioning the minimal AWS infrastructure to run the ELK based logging infrastructure.
  3. Deploy dockerized WordPress based blogging application.
  4. Monitor the AWS resources and the blogging application using you ELK based centralised logging and monitoring infrastructure.
  5. For bonus points: Demonstrate your knowledge and understanding by preparing an insightful dashboard of your choice.

To make things simple, you can use the official WordPress Docker image to run a web application and monitor it using the centralised logging setup that you have built above.

# Specifications

Here are the specs that we would like you to use:
  - OS: Ubuntu Server 14.04 64-bit
  - App Server: Gunicorn/Nginx
  - Python: 2.7
  - Ansible
  - Docker 1.10
  - Wordpress official Docker image https://hub.docker.com/_/wordpress/
  - ElasticSearch
  - Logstash
  - Kibana

# Deliverables:
  A Git repo with 
  1. the Ansible playbook, 
  2. Dockerfiles and Docker compose files
  3. shell script(s)
  - Launch the AWS infrastructure with EC2 servers.
  - Begin the configuration management / bootstrapping of the server using Ansible.
  - Deploy the ELK stack.
  - Finally start the blogging app as a Docker process.