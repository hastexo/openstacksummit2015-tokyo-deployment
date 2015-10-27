What about
## Mirantis?
Note: 


<!-- .slide: data-background-image="images/mirantis-logo.svg" data-background-size="contain" -->


Default deployment stack
## Fuel
## Puppet


Deployment checklist
# 1
### Install Fuel Master node


<!-- .slide: data-background-image="https://docs.mirantis.com/openstack/fuel/fuel-7.0/_images/fuelmenu_Network_Setup.png" data-background-size="contain" -->
Note: Download ISO, install to bare metal from ISO, boot up, set
certain settings in a BIOS-like interface. Some settings like DHCP,
DNS, NTP "should not be changed during the entire lifecycle of Fuel.


Deployment checklist
# 2
### Boot node servers
Note: "Node servers" is Fuel lingo for OpenStack nodes. They PXE-boot, and install Ubuntu 14.04. Support for CentOS 6 OpenStack nodes was removed in Fuel 7. 


<!-- .slide: data-background-image="https://docs.mirantis.com/openstack/fuel/fuel-7.0/_images/fuel-dashboard01.png" data-background-size="contain" -->


## Plugins
Note: Mirantis provides extended functionality via the use of plugins,
which can be community-contributed.


<!-- .slide: data-background-image="https://docs.mirantis.com/openstack/fuel/fuel-7.0/_images/plugins-tab.png" data-background-size="contain" -->
Note: Functionality exposed via plugins includes
- FWaaS
- Juniper Contrail L2 support
- Mellanox ConnectX-3 SR-IOV support
- ELK
- SolidFire Cinder support


## Upgrades
Note: Supported from 6.1 (plus all upgrades) to 7.0. Upgrade process:
- download upgrade tarball,
- unpack manually (lrzuntar, needs 2GB RAM)
- run upgrade shell script (30-60 minutes)
- brief API outages during upgrade
- then deploy new OpenStack release