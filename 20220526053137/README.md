# Enable dropped or denied packets log for firewalld

## Editing the config file
Open the firewalld configuration file under
```/etc/firewalld/firewalld.conf```, and chage the value of
```LogDenied``` option. If LogDenied is enabled, logging rules are added right before the reject and drop rules in the INPUT, FORWARD and OUTPUT chains for the default rules and also the final reject and drop rules in zones. 

Possible values for ```LogDenied```:
1. all
1. unicast
1. broadcast
1. multicast
1. off

With the unicast, broadcast, and multicast setting, the pkttype match is used to match the link-layer packet type. With all, all packets are logged. 

## using ```firewall-cmd``` command
```bash
firewall-cmd --get-log-deined
firewall-cmd --set-log-deined=all
```

Tags:
```
#Linux #firewall #firewalld #log #logdenied #firewall-cmd
```

Related:
```
* https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/7/html/security_guide/configuring_logging_for_denied_packets
```
