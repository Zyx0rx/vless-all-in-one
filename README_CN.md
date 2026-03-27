# vless-all-in-one

[English](./README.md) | [简体中文](./README_CN.md)

Linux 服务器一体化代理部署脚本。

它可以帮助你快速部署和管理多种协议，包括 **VLESS**、**VMess**、**Trojan**、**Hysteria2**、**TUIC**、**NaiveProxy**、**Snell**、**SOCKS5** 和 **SS2022**。

## 文档

- **网站文档：** https://docs.vaiox.de/
- **Telegram 群组：** https://t.me/vless_vaio
- **Telegram 频道：** https://t.me/vaio_channel

## 赞助与推荐

### VPS / 服务器赞助商

<p>
  <a href="https://www.takehost.biz/" target="_blank" rel="noopener noreferrer">
    <img src="https://www.takehost.biz/favicon.ico" alt="takehost" width="50" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>takehost</strong>
  </a>
  — 提供独立服务器、VPS 和游戏服务器，网络峰值可达 100 Gbps。
</p>

<p>
  <a href="https://akile.io/register?aff_code=b349580b-113a-4b42-ab76-c2db81c5c22d" target="_blank" rel="noopener noreferrer">
    <img src="https://akile.io/favicon.ico" alt="AkileCloud" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>AkileCloud</strong>
  </a>
  — 多地区覆盖 / 解锁流媒体 / 提供多国 SOCKS5 落地出口 / 包含原生家宽 IP / 高性价比。
</p>

<p>
  <a href="https://cloud.yt.net/?ref=13192" target="_blank" rel="noopener noreferrer">
    <img src="https://cloud.yt.net/logo.png" alt="YT.NET" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>YT.NET</strong>
  </a>
  — 原生 IP / 送 CNIX NAT 入口 / 深港节点 / BGP 国际网络。
</p>

<p>
  <a href="https://dash.lain.sh?ref=Charonlio" target="_blank" rel="noopener noreferrer">
    <img src="https://dash.lain.sh/img/favicon-16x16.png" alt="Lain.sh" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>Lain.sh</strong>
  </a>
  — 原生 IP / 解锁流媒体 / 家宽 ISP / 独立服务器。
</p>

<p>
  <a href="https://www.cstonecloud.com/aff.php?aff=358" target="_blank" rel="noopener noreferrer">
    <img src="https://www.cstonecloud.com/logo.png" alt="CstoneCloud" height="15" style="vertical-align: middle; margin-right: 6px;" />
    <strong>CstoneCloud</strong>
  </a>
  — 住宅双 ISP / 解锁流媒体 / 直连 & 五网回程 9929 / CN2 双向接入。
</p>

<p>
  <a href="https://www.skylineconnect.io/signup?aff=01CC63AP" target="_blank" rel="noopener noreferrer">
    <img src="https://www.skylineconnect.io/images/favicon.svg" height="50">
    <strong>SkylineConnect</strong>
  </a>
  — 软银 / Lumen / 大陆优化 / 大流量服务器 / 虚拟机 10Gbps 网口。
</p>

<p>
  <a href="https://www.geelinx.com/aff/HLGCSMDN" target="_blank" rel="noopener noreferrer">
    <img src="https://www.geelinx.com/favicon.ico" alt="Geelinx" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>Geelinx</strong>
  </a>
  — 解锁流媒体 / 大陆优化 / 单向带宽计费。
</p>

### 指纹浏览器推荐

<p>
  <a href="https://roxybrowser.com?code=0128SUFA" target="_blank" rel="noopener noreferrer">
    <img src="https://roxybrowser.com/favicon.ico" alt="RoxyBrowser" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>RoxyBrowser</strong>
  </a>
  — 多账号独立环境 / 多端同步 / 防关联检测 / 团队协作 / 浏览器指纹隔离 / 代理绑定 / AI 多账号管理。
</p>

### iOS SSH 客户端推荐

<p>
  <a href="https://apps.apple.com/us/app/careserver/id6474921250" target="_blank" rel="noopener noreferrer">
    <img src="https://nicejwin.github.io/CareServerWebSite/assets/img/logo.png" alt="CareServer" height="50" style="vertical-align: middle; margin-right: 6px;" />
    <strong>CareServer</strong>
  </a>
  — 服务器实时监控（CPU / 内存 / 磁盘）/ 容器管理（Docker / Podman）/ 端口转发（本地 / 远程 / 动态）/ SFTP 文件管理 / 代理功能（SOCKS / HTTP）/ 分组管理。
</p>

## 功能特性

- 一键安装与管理
- 支持多协议共存部署
- 适配 Debian、Ubuntu、CentOS 和 Alpine
- 基于 Xray + Sing-box 双核心架构
- 提供用户管理、路由、订阅与故障排查文档

## 快速安装

```bash
wget -O vless-server.sh https://raw.githubusercontent.com/Zyx0rx/vless-all-in-one/main/vless-server.sh && chmod +x vless-server.sh && ./vless-server.sh
```

## 文档入口

- [网站文档](https://docs.vaiox.de/)

## 用于流量统计的自定义 Sing-box 构建

从 **v3.5.2** 开始，**Hysteria2 / TUIC / AnyTLS** 的用户流量统计功能需要启用 `with_v2ray_api` 的自定义 Sing-box 构建。

默认的上游 Sing-box 二进制通常 **不包含** 此能力。

如果你需要使用 Sing-box 的流量同步 / 配额 / 到期等功能，请下载对应 GitHub Release 附件中的自定义 Sing-box，并替换当前的 `/usr/local/bin/sing-box`。

Release 附件中已提供安装说明：

- `README-sing-box-with-v2ray-api.md`

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Zyx0rx/vless-all-in-one&type=Date)](https://www.star-history.com/#Zyx0rx/vless-all-in-one&Date)
