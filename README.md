# Home Assistant Configs

Our [Home Assistant](https://home-assistant.io/) configuration files. `secrets.yaml` is kept in a private repo on its own.

Lots of integration and automation still required - [todo list](TODO.md).

Tested against version 0.35.3

## Deployment

This git repo is the source of truth, changes are made in a clone and then pushed to the local server using Ansible.

**Setting up a clone**

```
git clone git@github.com:natm/homeassistant-config.git
git clone git@github.com:natm/homeassistant-config-secrets.git
cd homeassistant-config
virtualenv venv
source venv/bin/activate
pip install git+git://github.com/ansible/ansible.git@devel
```

**Pushing configurations**

```
ansible-playbook -i deploy/hosts deploy/playbooks/ha.yml
```

## Running Home Assistant in Docker

`docker run --restart=always --name homeassistant -d -v /etc/homeassistant/config/:/config -v /etc/localtime:/etc/localtime:ro -p 127.0.0.1:8123:8123 
homeassistant/home-assistant`
