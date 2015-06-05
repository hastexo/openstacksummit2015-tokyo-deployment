What about
## upgrades?
Note: 


<!-- .slide: data-background-image="images/redhat-logo.svg" data-background-size="contain" -->
### Upgrades supported


<!-- .slide: data-background-image="images/redhat-logo.svg" data-background-size="contain" -->
### Semi-automatic


<!-- .slide: data-background-image="images/redhat-logo.svg" data-background-size="contain" -->
### Staggered service updates
Note: Control services first, then compute


<!-- .slide: data-background-image="images/ubuntu-logo.svg" data-background-size="contain" -->
### Upgrades supported
### `juju set`


<!-- .slide: data-background-image="images/ubuntu-logo.svg" data-background-size="contain" -->
### (Almost) fully automatic
```yaml
openstack-origin: cloud:trusty-kilo/updates
```


<!-- .slide: data-background-image="images/ubuntu-logo.svg" data-background-size="contain" -->
### Staggered service updates
Note: Control services first, then compute


<!-- .slide: data-background-image="images/suse-logo.svg" data-background-size="contain" -->
### Upgrades supported


<!-- .slide: data-background-image="images/suse-logo.svg" data-background-size="contain" -->
### Semi-automatic
### `suse-cloud-upgrade`


<!-- .slide: data-background-image="images/suse-logo.svg" data-background-size="contain" -->
### *"Stop the world"*
Note: For SUSE Cloud 4 to 5 upgrades, caveats apply:

- All instances must be suspended

- All API services are down for the upgrade

- Ceph nodes must migrate to SLES 12

- Hyper-V nodes must be reinstalled (meaning Hyper-V instances are lost and must be recreated)

- If `suse-cloud-upgrade` fails, support intervention is required

Reference: https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/data/sec_depl_maintenance_upgrade.html


<!-- .slide: data-background-image="images/rackspace-logo.svg" data-background-size="contain" -->
### Upgrades supported


<!-- .slide: data-background-image="images/rackspace-logo.svg" data-background-size="contain" -->
### Fully automatic
### `run-upgrade.sh`


<!-- .slide: data-background-image="images/rackspace-logo.svg" data-background-size="contain" -->
### No impact on VMs
