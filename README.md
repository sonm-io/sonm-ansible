sonm-ansible
============

This repo contains a bunch of an ansible scenarios to
deploy the components of the SONM network.

Install SONM network components:
```
ansible-playbook -i my_hosts install_sonm.yaml
```


Update components to the latest stable version:
```
ansible-playbook -i my_hosts install_sonm.yaml
```


Note! Config and keys updates are disabled by default. To enable it, you must pass the `update_config` variable and set it to True; It is reachable via `extra vars`, for example:

```
ansible-playbook -i hosts_office \
    --extra-vars "update_config=true update_keys=true" \
    update_sonm.yaml
```


### Roles included:

* common: useful stuff, locales, etc
* ansible-docker: latest docker runtime
* sonm-pkgcloud: configure SONM packagecloud repo
* sonm-keys: deploy Ethereum-keys for SONM network components
* sonm-client: install SONM Node and Cli
* sonm-worker: install SONM Worker (require Docker installed)
* sonm-dwh: install geth-node and DWH (ubuntu-only)
