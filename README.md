# Ansible Role: Firewall (iptables)

Installs an iptables-based firewall for Linux.


## Example Playbook

    - hosts: server
      vars_files:
        - vars/main.yml
      roles:
        - { role: dosh.firewall }

*Inside `vars/main.yml`*:

    firewall_allowed_tcp_ports:
      - "22"
      - "25"
      - "80"


