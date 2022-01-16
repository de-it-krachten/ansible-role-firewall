[![CI](https://github.com/de-it-krachten/ansible-role-firewall/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-firewall/actions?query=workflow%3ACI)


# ansible-role-firewall

Role to open firewall ports for incoming traffic.
Supports firewalld, ufw and iptables


Platforms
--------------

Supported platforms

- CentOS 7
- CentOS 8
- RockyLinux 8
- AlmaLinux 8
- Debian 10 (Buster)
- Debian 11 (Bullseye)
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS



Role Variables
--------------
<pre><code>
# List of posts to open
firewall_ports: []

# List of unsupported firewalls
firewall_type_unsupported:
  - nftables
</pre></code>


Example Playbook
----------------

<pre><code>
- name: sample playbook for role 'firewall'
  hosts: all
  vars:
    firewall_ports: [{'port': '22', 'proto': 'tcp'}, {'port': '53', 'proto': 'udp'}]
  tasks:
    - name: Include role 'firewall'
      include_role:
        name: firewall
</pre></code>
