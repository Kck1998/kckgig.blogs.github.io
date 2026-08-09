---
layout: default
title: Home
---

# Cibi's Network Lab

Welcome to my networking blog.

I document hands-on networking projects, troubleshooting experiences, configuration guides, and lessons learned while solving real-world network problems.

## Latest Project

### Configuring a TP-Link TD-W8968 as an Access Point for JioFiber

I recently faced an issue with my JioFiber router with 30mbps is not reaching ground floor in my house, where router is placed on the top floor, and sibling needs the data there. So, she keeps on recharging her mobile data. So, I've remembered that I have an older TP-Link TD-W8968 modem-router which purchases in 2015 where my high school got completed. 

Since I've started to learn networking, this sparks me into this to check the router can be used as access point. Those who do not know about access point see the references. 

So, having an older TP-Link TD-W8968 modem-router into an access point for my JioFiber network is that what I've thought to do.

The project involved:

- Understanding access-point and router modes
- Identifying two separate IPv4 networks
- Resolving a `169.252.x.x` automatic address
- Changing the TP-Link management address
- Disabling the TP-Link DHCP server
- Configuring a LAN-to-LAN connection
- Testing Wi-Fi and Ethernet connectivity
- Moving all devices onto one `192.168.25.x` network

The complete step-by-step guide is coming soon.

## Final Network Configuration

```text
JioFiber gateway: 192.168.25.x
TP-Link admin IP: 192.168.25.x
TP-Link DHCP: Disabled
Connection type: LAN-to-LAN
``
