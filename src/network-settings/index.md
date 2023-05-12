# Network Settings

Difuse offers a host of Network Settings to configure your network interfaces, routes, DHCP client options etc. In this page you can see a few of the terms used in the Network Settings and their definitions.

## LAN 
The LAN (Local Area Network) is the network that your router is connected to. This is the network that your devices will connect to and be assigned an IP address from. 

In Difuse you can configure DHCP on the LAN interface to automatically assign IPv4 addresses to devices that connect to your router and if needed you can assign static IPs to some or if not all the devices on your network. 

As far as IPv6 on the LAN interface goes, you can configure a static IPv6 address or you can use the SLAAC (Stateless Address Autoconfiguration) method to automatically assign IPv6 addresses to devices on your network or use other options that is available to you in the IPv6 tab of the LAN interface.

## WiFi

The WiFi interface is the wireless interface on your router. You can configure the WiFi interface to broadcast a WiFi network and configure the SSID, password, channel, bandwidth etc.

## WAN

The WAN (Wide Area Network) is the network that your router is connected to. This is the network that your router will connect to the internet through. We offer primarily 3 main options for both IPv4 and IPv6 on the WAN interface, they are:

- DHCP (both v4 and v6)
- Static IP
- PPPoE

You can select the appropriate option for your network and configure it accordingly.

## Routes

Routes are used to tell your router where to send traffic to. You can add routes to your router to tell it where to send traffic to for a specific network. There are primarily 3 types of routes that you can add to your router:

- Policy Based Routes
- Static IPv4 Routes
- Static IPv6 Routes

## DNS & DHCP

DNS (Domain Name System) is used to resolve domain names to IP addresses. You can configure the DNS servers that your router uses to resolve domain names. You can also configure the DHCP server on your router to assign DNS servers to devices that connect to your router.