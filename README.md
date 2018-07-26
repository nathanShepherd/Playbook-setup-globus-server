This playbook will install the Globus-Connect-Server software and prerequisite software. Then an endpoint will be initialized on the host. After running this playbook, globus-url-copy can be used in the commandline.

## Run the playbook with the following incantation in the command line:
```
ansible-playbook main.yml --user root --ask-pass
```
The on-screen prompts will ask for the name of the Endpoint to be created and whether it should be made public.

## Start the Globus Endpoint after running the Playbook
```
sudo globus-connect-server-setup
```
Authenticate Endpoint by entering a Globus ID and password

### If you do not have Ansible installed on your machine
```
sudo yum install ansible
```
