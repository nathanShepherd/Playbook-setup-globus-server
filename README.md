#Run the playbook with the following incantation in the command line:
```
ansible-playbook main.yml --user root --ask-pass
```
The on-screen prompts will ask for the name of the Endpoint to be created and whether it should be public.

#Start the Globus Endpoint after running the Playbook
```
sudo globus-connect-server-setup
```
