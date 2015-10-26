What about
## upgrades?
Note: 


<!-- .slide: data-background-image="images/redhat-logo.svg" data-background-size="contain" -->


<!-- .slide: data-background-image="https://media.giphy.com/media/ALvdHigd2gBqw/giphy.gif" data-background-size="cover" -->


<!-- .slide: data-background-image="images/ubuntu-logo.svg" data-background-size="contain" -->


### Upgrades supported
### `juju set`


### (Almost) fully automatic
```yaml
openstack-origin: cloud:trusty-liberty/updates
```


### Staggered service updates
Note: Control services first, then compute


<!-- .slide: data-background-image="images/suse-logo.svg" data-background-size="contain" -->


### Upgrades supported


### Semi-automatic
### `suse-cloud-upgrade`


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


### Fully automatic
### `run-upgrade.sh`


### No impact on VMs
