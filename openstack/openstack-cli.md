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

### List Total Amount of Floating IP
- openstack ip availability list

### List Servers running on current tenant.
- openstack server list

### List Servers running on all tenants.
- openstack server list --all-projects

### Delete server instance
- openstack server delete [ Instance ID ]
  - openstack server delete 2f82b081-8cda-4c24-baf0-884d64b34454

### Create server instance
- openstack server create --image <image> --flavor <flavor> --availability-zone nova:501d6571-2881-4beb-9ba7-c2f566ae9be5 --nic net-id=<network-id> <server-name>
