# overcloud-nova-domain

This playbook will change the default domain for instances in OpenStack.

This is meant to be run on the undercloud of a Red Hat OpenStack Platform deployment.

To run:

1. Edit the vars.yml file and set the nova_domain variable to your desired domain
2. Source your stackrc file on the undercloud

  ```$ source ~/stackrc```

3. Run the playbook

   ```$ ansible-playbook -i /usr/bin/tripleo-ansible-inventory change_nova_dhcpdomain.yml```
