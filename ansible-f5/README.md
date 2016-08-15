F5 playbook
====================================
This Ansible Role will deploy, destroy, and modify load balancing pools connected to an F5 Load Balancer
The hosts file needs to be customized for the environment.
Make sure to update the vault variable with f5_password so that the admin password gets loaded
The following variables will need to be declared:

admin_user


When creating a new pool:
load_balancer_method
pool_name

When deleting a pool:
pool_name

When adding or removing a node to a pool:
node_host
port

There are four roles with this playbook:
f5_create_pool
f5_modify_pool
f5_delete_pool
f5_add_node
f5_remove_node

Set the hosts file for the appropriate role in the hosts file or in the collection, update pass in or update variables as appropriate, and run the playbook

