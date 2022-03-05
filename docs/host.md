# HOST Config

## NetworkManager

File: /etc/NetworkManager/conf.d/00-use-dnsmasq.conf

```
# /etc/NetworkManager/conf.d/00-use-dnsmasq.conf
# Use dnsmasq plugin of NetworkManager.
#
[main]
dns=dnsmasq
```
File: /etc/NetworkManager/dnsmasq.d/01-use-local-dns.conf

```
# /etc/NetworkManager/dnsmasq.d/01-use-local-dns.conf
# see
# https://itectec.com/ubuntu/ubuntu-how-to-add-dnsmasq-and-keep-systemd-resolved-18-04/
#
interface=lo
bind-interfaces
listen-address=127.0.0.1

```

File: /etc/NetworkManager/dnsmasq.d/02-dns-servers.conf

```
# /etc/NetworkManager/dnsmasq.d/02-dns-servers.conf
#
# DNS Server
server=1.0.0.1
server=1.1.1.1
server=8.8.8.8

```

File: /etc/NetworkManager/dnsmasq.d/10-test-domain.conf

```
# /etc/NetworkManager/dnsmasq.d/10-test-domain.conf
#
# local webdev .test domains
address=/.test/127.0.0.1
```
