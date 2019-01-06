# Test

This test project is ansible role which will install openvpn client on Ubuntu 16.04. and do configure it. 

Created during test ececution for [**Baikalteam company**](http://www.baikalteam.com)

# Features
It should d ochanges only on Ubuntu 16.04. (xenial ) by terms of test task. All tasks implemented in single role.  Role behavior one of two ways:
1. Initial service configuration
2. Checkout of configuration and does correct configuration if it needs

# Variables
| **Name**                          | **Default**                                                       | **Description**                                                                                            |
|:------------------------------|:--------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------|
| openvpn_version               | 2.3.11                                                        | Version of OpenVPN to install                                                                          |

# Author 
(C) Rinat Ametov


