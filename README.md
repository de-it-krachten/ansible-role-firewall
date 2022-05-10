[![CI](https://github.com/de-it-krachten/ansible-role-firewall/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-firewall/actions?query=workflow%3ACI)


# ansible-role-firewall

Role to open firewall ports for incoming traffic.
Supports firewalld, ufw and iptables


Platforms
--------------

Supported platforms

- Red Hat Enterprise Linux 7<sup>1</sup>
- Red Hat Enterprise Linux 8<sup>1</sup>
- CentOS 7
- RockyLinux 8
- AlmaLinux 8<sup>1</sup>
- Debian 10 (Buster)
- Debian 11 (Bullseye)
- Ubuntu 18.04 LTS
- Ubuntu 20.04 LTS
- Ubuntu 22.04 LTS

Note:
<sup>1</sup> : no automated testing is performed on these platforms

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
