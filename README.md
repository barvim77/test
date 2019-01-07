# Test

This test project is ansible role which will install ***openvpn client*** on 
**Ubuntu 16.04.** and do configure it.

Created during test ececution for 
[**Baikalteam company**](http://www.baikalteam.com)

# Features
It should do changes only on Ubuntu 16.04. (xenial ) by terms of test task. 
All tasks implemented in single role.  Role's behavior assumes one of two ways:
1. Initial service configuration
2. Checkout of configuration and does correct configuration if it needs

# Variables
| **Name**   | **Default**     | **Description**|
|:---------|:------------|:------------|
|openvpn_ca_certificate|<example config hardcoded>||
|openvpn_certificate|<example config hardcoded>|OpenVPN certificate|
|openvpn_distribution_release|xenial|Name of distribution release allowed|
|openvpn_distribution_version|16.04|Version of distribution release allowed|
|openvpn_private_key|<example config hardcoded>|OpenVPN private key|
|openvpn_remote_host|8.8.8.8|OpenVPN client remote host|
|openvpn_remote_port|2195|OpenVPN client remote port|
|openvpn_remote_prot|udp|OpenVPN client protocol|
|openvpn_static_key|<example config hardcoded>|OpenVPN secret static key|


# Tags
Use --tags [Tagname] to enable/disable parts of tasks. On default all tasks are enabled, but if you used at once single tag, then unicluded tagged tasks will be disabled.

| **Tagname**   | **Description**|
|:---------|:------------|
| **update**  | Enable updating of all apt repository|
|**install_openvpn**|Enable openvpn client installation|



# Running test task
Use **test.sh** shell script or run **"sudo ansible-playbook ./test.yml"** from test 
directory

# Author
(C) Rinat Ametov


