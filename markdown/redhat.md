<!-- .slide: data-background-image="images/redhat-logo.svg" data-background-size="contain" -->


<!-- .slide: data-background-image="https://cinemaautopsy.files.wordpress.com/2013/04/never-ending-story.jpeg" data-background-size="cover" -->


Default deployment stack
## Packstack
## Puppet
# Nope <!-- .element: class="fragment stamp" -->


Default deployment stack
## Foreman
## Puppet
# Nope <!-- .element: class="fragment stamp" -->


Default deployment stack
## OSP Director
## TripleO
# Maybe? <!-- .element: class="fragment stamp" -->


<!-- .slide: data-background-iframe="https://www.redhat.com/en/about/press-releases/red-hat-acquire-it-automation-and-devops-leader-ansible" data-background-size="contain" -->


Deployment checklist
# 1
### Install Director node


Create
## Director user


Create
## image
and
## template
directories


## Register
with RHSM


Enable software
## repositories


Install
## Director packages
```bash
sudo yum install -y python-rdomanager-oscplugin
```
Note: this is actually pretty neat. Your installer is just a plugin
for the generic `openstack` client.


## Configure Undercloud


Fetch & install
## Overcloud images


Deployment checklist
# 2
### Install Overcloud


<!-- .slide: data-background-image="https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux_OpenStack_Platform/7/html/Director_Installation_and_Usage/images/Diagram-002-Network.png" data-background-size="contain" -->


Overcloud
### Installation options


## Test Overcloud
Web UI (Tuskar)


## Basic Overcloud
CLI only
Note: CLI is `openstack baremetal` or `ironic`.


## Advanced Overcloud
CLI only
Note: Advanced overcloud includes Ceph storage, and HA node fencing.
