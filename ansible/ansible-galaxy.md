# Ansible Galaxy Cheatsheet

## Permissions Error while running `ansible-galaxy`
### Problem:
- extracting network_interface to /etc/ansible/roles/network_interface
 [WARNING]: - network_interface was NOT installed successfully: Could not update files in /etc/ansible/roles/network_interface: [Errno 13] Permission denied:
'/etc/ansible/roles/network_interface'

ERROR! - you can use --ignore-errors to skip failed roles and finish processing the list.

### Solution:
- cd into the location of your playbook or roles directory
- use -p or --roles-path options to set your own roles path.

#### Example:
 ansible-galaxy install -r requirements.yml -p ./roles/

#### Docs:
http://docs.ansible.com/ansible/latest/intro_configuration.html#roles-path
man ansible-galaxy
-p ROLES_PATH, --roles-path=ROLES_PATH
           The path to the directory containing your roles. The default is the roles_path configured in your ansible.cfg file (/etc/ansible/roles if not configured)
