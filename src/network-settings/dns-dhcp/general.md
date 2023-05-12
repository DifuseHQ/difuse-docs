# Network Settings - DNS & DHCP - General

The general page offers a few options to configure the DNS & DHCP settings, let's go over all of them:

<a data-fancybox data-src="./img/1.png" data-caption="Network Settings - DNS & DHCP - General">
  <img src="./img/1.png" />
</a>

## Domain Requirement

If this option is turned on, the underlying dnsmasq service will not query the upstream DNS server for domain names that are not valid FQDN’s

## DHCP Authority

This option will set the DHCP server running inside your device as the only one in the network, if you have another DHCP server that is running in authoritative mode you can turn this off here.

## Service Domain

The DNS service running on the device will only accept DNS requests from the local subnet, it's usually a good idea to keep this on.

## Filtering Responses

Some ISPs provide IPv6/IPv4 without routing enabled, in that case you can filter the responses returned by the built-in DNS server to exclude A/AAAA responses.

## DNS Forwardings

By default there are some forwardings setup that will help proxying your DNS requests to a DNS-over-HTTPS proxy, and also blocking out some DoH servers that are used by Apple/Mozilla so that all clients in the network is forced to use our DNS server, keeping this options the way it is is also important for Content Filtering & Adblock.

