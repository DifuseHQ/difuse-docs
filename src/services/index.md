# Services

Difuse provides a bunch of services that can be used within the network. Here's all of them:

## ACME Certificates

ACME Certificates is a service that allows you to generate SSL certificates for your domains. It uses [Let's Encrypt](https://letsencrypt.org/) as a certificate authority.

## Adblock & Content Filtering

Adblock & Content Filtering is a service that allows you to block ads and other unwanted content on your network. It uses the built-in DNS server to block domains. We also provide custom list of domains to block in their own categories.

## Cloudflare Tunnels

Cloudflare Tunnels is a service that allows you to expose your local services to the internet using [Cloudflare Argo Tunnels](https://developers.cloudflare.com/cloudflare-one/connections/connect-apps). It's a really good choice if you're behind a CGNAT or don't want to expose your IP address to the internet. This also provides protection via the cloudflare web application firewall (WAF).

## Storage

Storage is a service that allows you to create a NAS (Network Attached Storage) on your network. It uses [Samba](https://www.samba.org/) to provide SMB shares, you can mount USB drives or use the built-in storage (if you have a device with the M.2 SSD).

## Dynamic DNS

Dynamic DNS is a service that allows you to create a domain name that points to your public IP address. We support upto 70 different providers, so you can choose the one that you prefer.

## Intrusion Prevention

Intrusion Prevention is a service that automatically blocks bad peers from trying to authenticate to critical services over and over again, think of it like a simpler version of fail2ban. It currently supports 3 services, namely: SSH, Asterisk and the Difuse GUI.

## IPFS

IPFS is a service that allows you to create a local IPFS node on your network. It uses [kubo](https://github.com/ipfs/kubo) to provide a web interface to manage your node.

## WireGuard VPN

WireGuard VPN is a service that allows you to create a VPN server on your network. It uses [WireGuard](https://www.wireguard.com/) to provide a secure connection to your network. You can also use it to connect to other WireGuard servers.