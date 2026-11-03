# Tencent & WeChat Direct Rules for PassWall / Proxy

本项目收录并定期整理腾讯、微信、QQ、企业微信及腾讯云相关的核心公网 IP 网段（CIDR）与直连域名列表，适用于 OpenWrt PassWall、Clash、Sing-box 等代理工具的直连（Bypass）分流规则。

## 📊 文件说明

- **[tencent-ip.txt](./tencent-ip.txt)**：精简去重后的腾讯系 CDN、云服务及边缘节点 IP/CIDR 网段，支持大网段收拢与按 IP 升序排列。
- **[tencent-domain.txt](./tencent-domain.txt)**：适用于 PassWall / 域名白名单的纯根域名直连列表（已自动递归覆盖所有子域名，如 `qq.com` 自动覆盖 `weixin.qq.com` 等）。

## 🚀 使用方法

1. 克隆或下载本仓库中的 `tencent-ip.txt` 和 `tencent-domain.txt`。
2. 在 PassWall（或其他路由器代理插件）的**自定义直连 IP / CIDR 列表**中导入 `tencent-ip.txt`。
3. 在**直连域名列表 / 白名单**中导入 `tencent-domain.txt`。
