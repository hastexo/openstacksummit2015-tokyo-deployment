<!-- .slide: data-background-image="images/suse-logo.svg" data-background-size="contain" -->
### SUSE OpenStack Cloud 5 <!-- .element class="fragment" -->


Default deployment stack
## Crowbar
## Chef
Note: Reference: https://www.suse.com/documentation/suse-cloud-5/singlehtml/book_cloud_deploy/book_cloud_deploy.html


Deployment checklist
# 1
### Install Admin node


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/yast_crowbar_user.png" data-background-size="contain" -->


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/yast_crowbar_repos.png" data-background-size="contain" -->


```sh
screen install-suse-cloud
```


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_node_dashboard_initial.png" data-background-size="contain" -->


Don't like that?


Enter
## SUSE Studio


<!-- .slide: data-background-iframe="https://susestudio.com/a/Mrr6vv/suse-openstack-cloud-4-admin--2" data-background-size="contain" -->
# Alas, <!-- .element class="fragment" -->
### no SUSE Cloud 5 <!-- .element class="fragment" -->


Deployment checklist
# 2
### Install cloud nodes


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_node_dashboard_initial_nodes.png" data-background-size="contain" -->


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_node_dashboard_groups_initial.png" data-background-size="contain" -->


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_node_edit.png" data-background-size="contain" -->


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_node_bulk_edit_allocate.png" data-background-size="contain" -->


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_node_dashboard_groups_installed.png" data-background-size="contain" -->


### `crowbar_register`
Registers **existing** nodes for SUSE Cloud deployment


Deployment checklist
# 3
### Deploy OpenStack services


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_barclamp_nova_node_deployment.png" data-background-size="contain" -->
Note: Example deployment with Crowbar, showing Nova barclamps


<!-- .slide: data-background-image="https://www.suse.com/documentation/suse-cloud-5/book_cloud_deploy/graphics/depl_barclamp_pacemaker_node_deployment.png" data-background-size="contain" -->
Note: Example deployment with Crowbar, showing Pacemaker clusters
