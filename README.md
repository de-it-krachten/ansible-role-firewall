[![CI](https://github.com/de-it-krachten/ansible-role-firewall/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-firewall/actions?query=workflow%3ACI)


# ansible-role-firewall

Role to open firewall ports for incoming traffic.
Supports firewalld, ufw, iptables and Windows firewall



## Dependencies

#### Roles
- deitkrachten.firewalld
- deitkrachten.iptables
- deitkrachten.ufw

#### Collections
- ansible.posix
- community.general
- community.windows

## Platforms

Supported platforms

- Red Hat Enterprise Linux 8<sup>1</sup>
- Red Hat Enterprise Linux 9<sup>1</sup>
- RockyLinux 8
- RockyLinux 9
- OracleLinux 8
- OracleLinux 9
- AlmaLinux 8
- AlmaLinux 9
- SUSE Linux Enterprise 15<sup>1</sup>
- openSUSE Leap 15
- Debian 11 (Bullseye)
- Debian 12 (Bookworm)
- Ubuntu 20.04 LTS
- Ubuntu 22.04 LTS
- Ubuntu 24.04 LTS
- Fedora 40
- Fedora 41
- Windows Server 2012 R2<sup>1</sup>
- Windows Server 2016<sup>1</sup>
- Windows Server 2019<sup>1</sup>
- Windows Server 2022<sup>1</sup>

Note:
<sup>1</sup> : no automated testing is performed on these platforms

## Role Variables
### defaults/main.yml
<pre><code>
# List of posts to open
firewall_ports: []

# List of unsupported firewalls
firewall_type_unsupported:
  - nftables

# name of the windows firewall service
firewall_win_service_name: mpssvc
</pre></code>




## Example Playbook
### molecule/default/converge.yml
<pre><code>
- name: sample playbook for role 'firewall'
  hosts: all
  become: 'yes'
  vars:
    firewall_ports:
      - name: SSH
        port: '22'
        proto: tcp
      - name: DNS
        port: '53'
        proto: udp
  tasks:
    - name: Include role 'firewall'
      ansible.builtin.include_role:
        name: firewall
</pre></code>
