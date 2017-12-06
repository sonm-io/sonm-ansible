sonm-ansible
============

This repo contains a bunch of an ansible scenarios to
deploy the components of the SONM network.


TODO:

- [x] prepare environment
    - [x] add ssh-keys
    - [x] set-up system locales
    - [x] install common stuff (htop, mc, git, etc)
    - [x] install runtime dependencies (docker, ipvs, stun-server, etc) 

- [ ] deliver the SONM Network components
    - [x] Hub
    - [x] Worker
    - [x] Client's Node
    - [ ] Locator
    - [ ] Marketplace

Extra role to preparing build env:
- [ ] install the following packages:
    - git
    - go1.9
    - opencl-headers
    - nvidia-opencl-dev
    - debhelper
    - devscripts
    - dh-systemd

