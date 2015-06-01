Testing the playbook locally
============================
```
vagrant up
ansible-playbook -i inventory/vagrant_pre --private-key=~/.vagrant.d/insecure_private_key -u vagrant playbook/main.yml
```

You will have to use the inventory/vagrant_post hosts file after running the playbook the first time.


ansible-playbook -i path/to/inventory/file --private-key=ssh_key_location -u username playbook/main.yml