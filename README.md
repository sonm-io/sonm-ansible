sonm-ansible
============

This repo contains a bunch of an ansible scenarios to
deploy the components of the SONM network.

Note! Config updates are disabled by default. To enable it, you must pass the `update_config` variable and set it to True; It is reachable via `extra vars`, for example:

```
ansible-playbook -i hosts_office --extra-vars "update_config=true" update_sonm.yaml
```

Testing scenarios:

- [x] Deploy all parts to the one machine
- [x] Deploy each part to a different machines
- [x] Deploy multiple Workers for the one Hub
- [ ] Deploy multiple Hubs with cluster enabled (let's google for a consul role for the ansible)


TODO:

- [x] prepare environment
    - [x] add ssh-keys
    - [x] set-up system locales
    - [x] install common stuff (htop, mc, git, etc)
    - [x] install runtime dependencies (docker, ipvs, stun-server, etc) 

- [x] deliver the SONM Network components
    - [x] Hub
    - [x] Worker
    - [x] Client's Node
    - [x] Locator
    - [x] Marketplace
    - [x] Eth keys

Extra role to preparing build env:
- [ ] install the following packages:
    - git
    - go1.9
    - opencl-headers
    - nvidia-opencl-dev
    - debhelper
    - devscripts
    - dh-systemd

