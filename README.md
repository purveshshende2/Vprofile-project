# Vprofile-project

Prerequisite
VPROFILE PROJECT SETUP
1. Oracle VM Virtualbox
2. Vagrant
3. Vagrant plugins
    - a. vagrant plugin install vagrant-hostmanager
4. Git bash or equivalent editor


VM SETUP
1. Clone source code.
2. Cd into the repository.
3. Switch to the main branch.

Bring up vm’s
$ vagrant up

NOTE: Bringing up all the vm’s may take a long time based on various factors. If vm setup stops in the middle run “vagrant up” command again.
INFO: All the vm’s hostname and /etc/hosts file entries will be automatically updated.


PROVISIONING 
Services 

Services 
- Nginx (web sevice)
- Tomcat (Application server)
- RabbitMQ (Broker/Queuing Agent )
- Memcached (DB Caching )
- ElasticSearch (Indexing/Search service )
- MySQL (SQL Database)

Setup should be done in below mentioned order 
- MySQL (Database SVC) Memcache (DB Caching SVC)
- Memcache (DB Caching SVC)
- RabbitMQ (Broker/Queue SVC) 
- Tomcat (Application SVC) 
- Nginx (Web SVC) 
