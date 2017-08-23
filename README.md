# jenkins-up

Ansible provisioning for jenkins.smithmicro.io!


## Provisioning

Use "centos" user for initial setup with clean CentOS 7 box:

    ansible-playbook -u centos -i inventory.ini jenkins-server.yml

When rolling out updates to production, use your own account:

    ansible-playbook -u vtepliuk -i inventory.ini jenkins-server.yml


## Contributing

Use the Vagrantfile to try out your changes locally before opening a pull request:

    vagrant up --provision

    vagrant ssh

