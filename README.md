# Home Assistant Configs

Our [Home Assistant](https://home-assistant.io/) configuration files.

## Development & deployment

This git repo is the source of truth, changes are made in a clone and then pushed to the local server using Ansible.

**Setting up a clone**

```
git clone git@github.com:natm/homeassistant-config.git
cd homeassistant-config
virtualenv venv
source venv/bin/activate
pip install git+git://github.com/ansible/ansible.git@devel
```

**Pushing configurations**

```
ansible-playbook -i deploy/hosts deploy/playbooks/ha.yml
```
