# clusterworks

Ansible playbooks for OpenHPC recipies

## Quick Start

1. Clone or fork this repository
2. Copy the template config file to `config.yml` and edit as required
3. Add machines to the inventory
4. Run `./run_playbook.sh install_master`
5. Run `./run_playbook.sh install_nodes`
6. Boot up all the nodes
7. Run `./run_playbook.sh update_nodes`

## Software Stack status

- [x] CentOS / RedHat
- [ ] SLES
- [x] xCAT Stateful
- [x] xCAT Stateless
- [ ] Warewulf
- [x] PBS Professional
- [ ] Slurm

## Proxy support

This playbook supports two kinds of proxies.

Firstly, set `proxy_host` and `proxy_port` in the config file to set an upstream proxy to download assets required from the Internet.

Secondly, set `repository_type == 'cache'` in order to deploy a local Squid proxy on the SMS node in order to cache packages for worker node deployment.
If you also use a proxy to connect to the internet, set it as above and it will be configured as the upstream peer for the local cache.

## License

GPLv3
