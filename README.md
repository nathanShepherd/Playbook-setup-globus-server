This playbook will install the Globus-Connect-Server software and prerequisite software. Then an endpoint will be initialized on the host. After running this playbook, globus-url-copy can be used in the commandline.

## Run the playbook in the command line
```
ansible-playbook main.yml --user root --ask-pass --extra-vars "endpoint_name=NAME is_public=True
```

Variables set at runtime include:
- endpoint_name: defaults to 'NAME', name for globus endpoint (Seperate from hostname)
- is_public : defaults to 'False', whether to publish results to globus (does not affect test)

## Start the Globus Endpoint after running the Playbook
```
sudo globus-connect-server-setup
```
Authenticate Endpoint by entering a Globus ID and password

### If you do not have Ansible installed on your machine
```
sudo yum install ansible
```
