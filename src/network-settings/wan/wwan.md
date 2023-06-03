# Network Settings -  WWAN

```admonish info
This section is only applicable to you if you have a WWAN module in your system.
```

<a data-fancybox data-src="./img/7.png" data-caption="Network Settings - WAN - WWAN">
  <img src="./img/7.png" />
</a>


## APN & PIN

The WWAN connection usually doesn’t require any sort of configuration as the setup is done automatically. If your service provider requires an APN that needs to be setup or if your SIM card that is inserted has a PIN you can specify them here.

## PDP Type

If your ISP is finicky about IPv6 or you're having issues multi-homing IPv6 with your main WAN interface in *any* way, you can always choose IPv4 only as the PDP type. This will force the WWAN interface to only use IPv4.

## IPv6 Prefix Delegation

If your ISP provides you with an IPv6 prefix delegation that you want to use on your LAN, you can enable this option, if you don't want your LAN to use IPv6, you can disable it.