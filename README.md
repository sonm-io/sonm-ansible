sonm-ansible
============

This repo contains a bunch of an ansible scenarios to
deploy the components of the SONM network.


TODO:

- [ ] prepare environment
    - [ ] add ssh-keys
    - [ ] set-up system locales
    - [ ] install common stuff (htop, mc, git, etc)
    - [ ] install runtime dependencies (docker, ipvs, stun-server, etc) 

- [ ] deliver the SONM Network components
    - [ ] rsync'ing packages from the local repo (just a directory with a *.deb's)
    - [ ] set-up configs (override defaults with values from a host_vars)
