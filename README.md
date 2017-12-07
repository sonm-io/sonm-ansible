sonm-ansible
============

This repo contains a bunch of an ansible scenarios to
deploy the components of the SONM network.

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

