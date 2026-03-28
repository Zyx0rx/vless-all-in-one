# vless-all-in-one

[English](./README.md) | [简体中文](./README_CN.md)

An all-in-one proxy deployment script for Linux servers.

It helps you quickly deploy and manage multiple protocols in one place, including **VLESS**, **VMess**, **Trojan**, **Hysteria2**, **TUIC**, **NaiveProxy**, **Snell**, **SOCKS5**, and **SS2022**.

## Documentation

- **Website:** https://docs.vaiox.de/
- **Telegram Group:** https://t.me/vless_vaio
- **Telegram Channel:** https://t.me/vaio_channel

## Sponsors & Recommendations

### Hosting Sponsors

<p>
  <a href="https://www.takehost.biz/" target="_blank" rel="noopener noreferrer">
    <img src="https://www.takehost.biz/favicon.ico" alt="takehost" width="50" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>takehost</strong>
  </a>
  — Dedicated servers, VPS, and game servers with up to 100 Gbps networking.
</p>

<p>
  <a href="https://akile.io/register?aff_code=b349580b-113a-4b42-ab76-c2db81c5c22d" target="_blank" rel="noopener noreferrer">
    <img src="https://akile.io/favicon.ico" alt="AkileCloud" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>AkileCloud</strong>
  </a>
  — Multi-region coverage, streaming-unlocked routes, multi-country SOCKS5 exit nodes, native residential IP options, and strong value for money.
</p>

<p>
  <a href="https://cloud.yt.net/?ref=13192" target="_blank" rel="noopener noreferrer">
    <img src="https://cloud.yt.net/logo.png" alt="YT.NET" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>YT.NET</strong>
  </a>
  — Native IP, complimentary CNIX NAT entry, Shenzhen–Hong Kong optimized routes, and a BGP international network.
</p>

<p>
  <a href="https://dash.lain.sh?ref=Charonlio" target="_blank" rel="noopener noreferrer">
    <img src="https://dash.lain.sh/img/favicon-16x16.png" alt="Lain.sh" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>Lain.sh</strong>
  </a>
  — Native IP, streaming-unlocked routes, residential ISP resources, and dedicated servers.
</p>

<p>
  <a href="https://www.cstonecloud.com/aff.php?aff=358" target="_blank" rel="noopener noreferrer">
    <img src="https://www.cstonecloud.com/logo.png" alt="CstoneCloud" height="15" style="vertical-align: middle; margin-right: 6px;" />
    <strong>CstoneCloud</strong>
  </a>
  — Residential dual-ISP connectivity, streaming-unlocked routes, direct connectivity and five-network 9929 return paths, plus dual CN2 access.
</p>

<p>
  <a href="https://www.skylineconnect.io/signup?aff=01CC63AP" target="_blank" rel="noopener noreferrer">
    <img src="https://www.skylineconnect.io/images/favicon.svg" height="50">
    <strong>SkylineConnect</strong>
  </a>
  — SoftBank/Lumen routes, mainland China optimized networking, high-traffic servers, and 10 Gbps virtual machine ports.
</p>

<p>
  <a href="https://www.geelinx.com/aff/HLGCSMDN" target="_blank" rel="noopener noreferrer">
    <img src="https://www.geelinx.com/favicon.ico" alt="Geelinx" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>Geelinx</strong>
  </a>
  — Streaming-unlocked routes, mainland China optimized networking, and one-way bandwidth billing.
</p>

### Recommended Fingerprint Browser

<p>
  <a href="https://roxybrowser.com?code=0128SUFA" target="_blank" rel="noopener noreferrer">
    <img src="https://roxybrowser.com/favicon.ico" alt="RoxyBrowser" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>RoxyBrowser</strong>
  </a>
  — Isolated multi-account environments, cross-device sync, anti-linking detection, team collaboration, browser fingerprint isolation, proxy binding, and AI-powered multi-account management.
</p>

### Recommended iOS SSH App

<p>
  <a href="https://apps.apple.com/us/app/careserver/id6474921250" target="_blank" rel="noopener noreferrer">
    <img src="https://nicejwin.github.io/CareServerWebSite/assets/img/logo.png" alt="CareServer" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>CareServer</strong>
  </a>
  — Real-time server monitoring (CPU, memory, disk), container management (Docker/Podman), port forwarding (local/remote/dynamic), SFTP file management, proxy support (SOCKS/HTTP), and group management.
</p>

## Features

- One-click installation and management
- Supports multiple protocols on the same server
- Built for Debian, Ubuntu, CentOS, and Alpine
- Xray + Sing-box dual-core architecture
- User management, routing, subscriptions, and troubleshooting docs

## Quick Install

```bash
wget -O vless-server.sh https://raw.githubusercontent.com/Zyx0rx/vless-all-in-one/main/vless-server.sh && chmod +x vless-server.sh && ./vless-server.sh
```

## Documents

- [Website Docs](https://docs.vaiox.de/)

## Sing-box custom build for traffic stats

Starting from **v3.5.3**, Sing-box user traffic statistics for **Hysteria2 / TUIC / AnyTLS** require a custom Sing-box build with `with_v2ray_api` enabled.

The default upstream Sing-box binary usually does **not** include this capability.

For users who need Sing-box traffic sync / quota / expiry workflows, download the custom Sing-box asset attached to the corresponding GitHub Release and replace your current `/usr/local/bin/sing-box` binary.

A step-by-step installation note is provided in the release asset:

- `README-sing-box-with-v2ray-api.md`

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Zyx0rx/vless-all-in-one&type=Date)](https://www.star-history.com/#Zyx0rx/vless-all-in-one&Date)
