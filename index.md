---
layout: default
title: Home
---

# Cibi's Network Lab

Welcome to my networking blog.

I document hands-on networking projects, troubleshooting experiences, configuration guides, and lessons learned while solving real-world network problems.

---

## 🚀 Latest Featured Project

### How I Configured a TP-Link TD-W8968 as an Access Point for JioFiber

<div class="badge-group">
  <span class="badge badge-blue">Hardware Reuse</span>
  <span class="badge badge-purple">Subnetting</span>
  <span class="badge badge-green">Verified Working</span>
</div>

I faced an issue with my 30 Mbps JioFiber connection not reaching the ground floor of my house, where the router is placed on the top floor. To solve this without purchasing new equipment, I repurposed an older **TP-Link TD-W8968 ADSL modem-router** from 2015 to act as a wireless access point and Ethernet switch.

<div class="callout callout-info">
  <div class="callout-title">📋 Key Project Highlights</div>
  <ul>
    <li>Understanding access-point vs router modes</li>
    <li>Eliminating Double NAT between two subnets</li>
    <li>Resolving <code>169.252.x.x</code> APIPA address issue</li>
    <li>Re-assigning TP-Link management IP & disabling DHCP</li>
    <li>Establishing a LAN-to-LAN uplink</li>
    <li>Consolidating all devices onto a single <code>192.168.25.x</code> subnet</li>
  </ul>
</div>

👉 **[Read the complete step-by-step guide →]({{ site.baseurl }}{% post_url 2026-08-09-tplink-td-w8968-jiofiber-access-point %})**

---

## ⚡ Final Verified Topology Quick Overview

<div class="card-grid">
  <div class="card">
    <div class="card-title">🌐 JioFiber Gateway</div>
    <p><code>192.168.25.1</code> (DHCP & NAT Active)</p>
  </div>
  <div class="card">
    <div class="card-title">📻 TP-Link Access Point</div>
    <p><code>192.168.25.2</code> (DHCP Disabled, LAN-to-LAN)</p>
  </div>
  <div class="card">
    <div class="card-title">💻 Unified Subnet</div>
    <p><code>192.168.25.x /24</code> (Single Broadcast Domain)</p>
  </div>
</div>
