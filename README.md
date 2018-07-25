Run the playbook with the following incantation:
```
ansible-playbook main.yml --user root --ask-pass
```

Start the Globus Endpoint after running the Playbook
```
sudo globus-connect-server-setup
```
