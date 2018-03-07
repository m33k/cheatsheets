# Openstack CLI Cheatsheet
## Openstack CLI is now the official way to manage openstack using the CLI. The old commands such as nova, glance, neutron, trove, etc. are now deprecated.

### List services on your Openstack Cluster
- openstack service list

### List hosts involved with your Openstack Cluster
- openstack host list

### List Floating IPs and projects they are assigned to.
- openstack floating ip list
- openstack floating ip show [ IP ]
  - provides details only on the ip argument passed.


### List Servers running on current tenant.
- openstack server list

### List Servers running on all tenants.
- openstack server list --all-projects

### Delete server instance
- openstack server delete [ Instance ID ]
  - openstack server delete 2f82b081-8cda-4c24-baf0-884d64b34454
