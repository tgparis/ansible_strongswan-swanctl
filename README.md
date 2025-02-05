# ansible_ipsec
Ansible that creates an IPSec configuration in the Swanctl config format.

## Instructions
Add host.
Run sudo ansible-playbook -i hosts main.yml

The swanctl formatted configuration file will be located in /etc/swanctl/conf.d/{{ parent_conn_name }}

## To Do
Add a bash script to parse the IP addresses from the swanctl.conf file(s) and then add those IPs to a VPN allow chain with IPTables.
