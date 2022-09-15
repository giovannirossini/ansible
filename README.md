# Ansible Playground

 <img src="https://docs.ansible.com/ansible/latest/_static/images/Ansible-Mark-RGB_White.svg" width="50">

This project is intended for studies and code sheet.

To start you need to create the SSH keys that will be used. To do this, run inside the project:

```shell
mkdir -p keys
ssh-keygen -t rsa -b 2048 -N '' -f keys/ansible_key
```

After creating the keys, you need to run the command:
```shell
docker-compose up -d
```

After the containers are up, you can access the "ansible server" through the command:
```shell
docker exec -it ansible sh
```

To put it into practice, just run the command:
```shell
ansible -m ping all
ansible-playbook examples.yml
```

