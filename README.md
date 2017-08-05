# Sysmgmt common role
This role will take care of the following on the nodes defined in the inventory file of the service.
- ntp
- resolv.conf


## Variables
The following variables will be used in the role and should be declared in the group_vars dir of the service:


~~~yaml
---
# DNS servers to use
nameservers:
  - 192.168.1.1
  - 8.8.8.8

# Domain to use
domain: l4rs.net

# DNS search list
domain_search_list: "l4rs.net"

# NTP time server
timeservers:
  - 0.centos.pool.ntp.org
  - 1.centos.pool.ntp.org
  - 2.centos.pool.ntp.org
  - 3.centos.pool.ntp.org
~~~
