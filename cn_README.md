[English](README.md) | **中文**

# Tailscale OpenWrt Binary Builder

## 中文说明

本项目每天自动检查 Tailscale 官方是否发布新版本。

当检测到新版本时，将自动：

1. 获取最新 Tailscale 源码
2. 编译适用于 OpenWrt 设备运行的二进制文件
3. 使用 UPX 进行压缩优化
4. 自动发布对应架构的构建产物

配合以下 LuCI 插件使用：

👉 https://github.com/whzhni1/luci-app-tailscale

即可实现 OpenWrt 设备端 Tailscale 二进制文件的在线自动更新。

### 功能特点

- 自动检测 Tailscale 新版本
- 自动编译 OpenWrt 可用二进制文件
- 自动使用 UPX 压缩
- 自动发布 GitHub Release
- 支持设备端在线更新
- 支持多种 OpenWrt 主流架构

### 支持架构

| 架构 | 包名 |
|-------------|---------|
| aarch64 | tailscale_*_linux-aarch64.tar.gz |
| armv5l | tailscale_*_linux-armv5l.tar.gz |
| armv6l | tailscale_*_linux-armv6l.tar.gz |
| armv7l | tailscale_*_linux-armv7l.tar.gz |
| i686 | tailscale_*_linux-i686.tar.gz |
| loongarch64 | tailscale_*_linux-loongarch64.tar.gz |
| mips-hardfloat | tailscale_*_linux-mips-hardfloat.tar.gz |
| mips-softfloat | tailscale_*_linux-mips-softfloat.tar.gz |
| mips64-hardfloat | tailscale_*_linux-mips64-hardfloat.tar.gz |
| mips64-softfloat | tailscale_*_linux-mips64-softfloat.tar.gz |
| mips64el-hardfloat | tailscale_*_linux-mips64el-hardfloat.tar.gz |
| mips64el-softfloat | tailscale_*_linux-mips64el-softfloat.tar.gz |
| mipsel-hardfloat | tailscale_*_linux-mipsel-hardfloat.tar.gz |
| mipsel-softfloat | tailscale_*_linux-mipsel-softfloat.tar.gz |
| powerpc64le | tailscale_*_linux-powerpc64le.tar.gz |
| riscv64 | tailscale_*_linux-riscv64.tar.gz |
| x86_64 | tailscale_*_linux-x86_64.tar.gz |

---

## 相关项目

- LuCI 插件：https://github.com/whzhni1/luci-app-tailscale

## 许可证

请参考 Tailscale 项目的许可证和使用条款。
