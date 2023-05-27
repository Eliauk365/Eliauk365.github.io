# 魔法上网一键脚本指南


# 前言

> - 风险提示：一键脚本使用存在风险，包括但是不限于系统被不安全的脚本入侵或病毒攻击。
> - 关于推荐指数：⭐⭐⭐⭐⭐ 为最高推荐，未知代表本人使用次数较少或者并未使用，并不代表脚本不能使用或者脚本存在问题。推荐指数仅代表个人观点，如果你有不同观点，以你为准，这里不讨论。

本次脚本收集尽可能的选择开源的一键脚本，有些脚本可能已经停止使用，但是仍然可以正常使用，有些脚本可能会存在系统兼容的问题，具体情况需要参考官方的一键脚本的使用文档。

本文只是作为收集整理，不对脚本的使用做任何保证。

# XRay一键脚本

## v2ray-agent

推荐指数：⭐⭐⭐⭐⭐

介绍：八合一共存脚本，支持：VLESS(TCP_Vision、Reality、gRPC、WS)、VMess(WS)、Trojan(TCP、gRPC)、Hysteria。

Github地址：[点击直达](https://github.com/mack-a/v2ray-agent)

脚本直达

```bash
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/mack-a/v2ray-agent/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
```

## Xray_onekey

推荐指数：⭐⭐⭐⭐

介绍：Xray 基于 Nginx 的 VLESS + XTLS 一键安装脚本

Github地址：[点击直达](https://github.com/wulabing/Xray_onekey)

脚本直达

```bash
# VLESS + TCP + TLS + Nginx + WebSocket
wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/wulabing/Xray_onekey/nginx_forward/install.sh" && chmod +x install.sh && bash install.sh

# VLESS + TCP + XTLS / TLS + Nginx
# VLESS + TCP + XTLS / TLS + Nginx 及 VLESS + TCP + TLS + Nginx + WebSocket 回落并存模式
wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/wulabing/Xray_onekey/main/install.sh" && chmod +x install.sh && bash install.sh
```

## multi-v2ray 

推荐指数：未知

介绍：这款软件支持Xray管理，同时也支持v2ray和xray相互独立。它的特点是不同命令(v2ray/xray)可以进入不同的core进行管理，从而实现了对不同协议的灵活控制。

Github地址：[点击直达](https://github.com/Jrohy/multi-v2ray)

脚本直达

```bash
# 安装命令
source <(curl -sL https://multi.netlify.app/v2ray.sh) --zh

# 升级命令(保留配置文件更新)
source <(curl -sL https://multi.netlify.app/v2ray.sh) -k

# 卸载命令
source <(curl -sL https://multi.netlify.app/v2ray.sh) --remove
```

# SingBox一键脚本

## sing-box-yes

推荐指数：未知

介绍：方便快捷的安装、管理sing-box💯

Github地址：[点击直达](https://github.com/FranzKafkaYu/sing-box-yes)

脚本直达

```bash
bash <(curl -Ls https://raw.githubusercontent.com/FranzKafkaYu/sing-box-yes/master/install.sh)
```

# V2Ray一键脚本

## V2Ray_ws-tls_bash_onekey

推荐指数：⭐⭐⭐⭐⭐

介绍：V2Ray_ws-tls_bash一键脚本，支持VMESS，VLESS。

Github地址：[点击直达](https://github.com/wulabing/V2Ray_ws-tls_bash_onekey)

脚本直达

```bash
# Vmess+websocket+TLS+Nginx+Website
wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/wulabing/V2Ray_ws-tls_bash_onekey/master/install.sh" && chmod +x install.sh && bash install.sh

# VLESS+websocket+TLS+Nginx+Website
wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/wulabing/V2Ray_ws-tls_bash_onekey/dev/install.sh" && chmod +x install.sh && bash install.sh
```

## 233boy-V2ray

推荐指数：未知

介绍：V2Ray 一键安装脚本 & 管理脚本

GitHub地址：[点击直达](https://github.com/233boy/v2ray)

脚本直达

```bash
bash <(wget -qO- -o- https://git.io/v2ray.sh)
```

# NaiveProxy一键脚本

## MisakaNo-NaiveProxy

推荐指数：未知

介绍：NaiveProxy 一键配置脚本

GitHub地址：[点击直达](https://github.com/Misaka-blog/naiveproxy-script)

脚本直达

```bash
wget -N --no-check-certificate https://raw.githubusercontent.com/Misaka-blog/naiveproxy-script/main/naiveproxy.sh && bash naiveproxy.sh
```

## naiveproxy-yg

**脚本作者存在争议，但该脚本暂无问题**

推荐指数：✨✨✨✨✨

介绍：naiveproxy-yg一键脚本，支持二维码显示，支持变更配置（多端口复用、自定义伪装网页，证书……）

GitLab地址：[点击直达](https://gitlab.com/rwkgyg/naiveproxy-yg)

脚本直达

```bash
wget -N https://gitlab.com/rwkgyg/naiveproxy-yg/raw/main/naiveproxy.sh && bash naiveproxy.sh
```

# Trojan-GO

## kenzok8-trojan-go一键二合一脚本

推荐指数：未知

介绍：Trojan onekey install shell Trojan && trojan.go一键脚本

GitHub地址：[点击直达](https://github.com/kenzok8/Trojan)

脚本直达

```bash
# vps上需要安装curl Ubuntu/Debian 系统安装 Curl 方法
apt-get update -y && apt-get install curl -y    
```

# Hysteria

## HI-HY

推荐指数：未知

介绍：Hello World！非钟国优化线路使用不佳？不想中转？hysteria一键搞定。

GitHub地址：[点击直达](https://github.com/emptysuns/Hi_Hysteria)

脚本直达

```bash
su - root #switch to root user.
bash <(curl -fsSL https://git.io/hysteria.sh)

# 首次安装后: hihy命令调出菜单,如更新了hihy脚本
```

# 带WEB界面一键脚本

## x-ui

推荐指数：⭐⭐⭐⭐⭐

介绍：支持单端口多用户、多协议的 xray 面板，究极缝合怪，通过免费的Telegram bot方便快捷地进行监控、管理你的代理服务

GitHub地址：[点击直达-魔改版](https://github.com/FranzKafkaYu/x-ui)

GitHub地址：[点击直达-原版](https://github.com/vaxilu/x-ui)

脚本直达

```bash
# ⚡从原版升级也可使用该命令，数据不会丢失⚡
bash <(curl -Ls https://raw.githubusercontent.com/FranzKafkaYu/x-ui/master/install.sh)
```

## Trojan Panel

推荐指数：未知

介绍：支持Xray/Trojan-Go/Hysteria/NaiveProxy的多用户Web管理面板

GitHub地址：[点击直达](https://github.com/trojanpanel)

脚本直达

```bash
source <(curl -L https://github.com/trojanpanel/install-script/raw/main/install_script.sh)
```

# 最后

如果你有好的脚本推荐，欢迎在评论区留言，我会及时添加到本文中。

**<center>人面不知何处去，桃花依旧笑春风</center>**

