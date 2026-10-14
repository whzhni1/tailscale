**English** | [中文](cn_README.md)

# Tailscale OpenWrt Binary Builder

This repository automatically checks for new official Tailscale releases every day.

When a new version is detected, the workflow will automatically:

1. Fetch the latest Tailscale source code
2. Build binaries optimized for OpenWrt
3. Compress binaries using UPX
4. Publish release artifacts for supported architectures

Designed to work together with:

👉 https://github.com/whzhni1/luci-app-tailscale

This enables automatic online updates of Tailscale binaries directly on OpenWrt devices.

### Features

- Daily Tailscale version monitoring
- Automatic binary compilation
- UPX compression for smaller package size
- Automatic GitHub Release publishing
- Online binary updates from OpenWrt devices
- Wide architecture support

### Supported Architectures

| Architecture | Package |
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

## Related Project

- LuCI App: https://github.com/whzhni1/luci-app-tailscale

## License

Please refer to the Tailscale project license and terms of use.
