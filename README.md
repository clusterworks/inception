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

## License

GPLv3
