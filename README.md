# openwrt-v2ray

V2Ray for OpenWrt

OpenWrt/LEDE 上可用的 V2Ray

[![Release Version](https://img.shields.io/github/release/rp-hello/openwrt-v2ray.svg)](https://github.com/rp-hello/openwrt-v2ray/releases/latest)
[![Latest Release Download](https://img.shields.io/github/downloads/rp-hello/openwrt-v2ray/latest/total.svg)](https://github.com/rp-hello/openwrt-v2ray/releases/latest)
[![Releases Download](https://img.shields.io/github/downloads/rp-hello/openwrt-v2ray/total.svg)](https://github.com/rp-hello/openwrt-v2ray/releases)

For luci-app-v2ray, please head to [luci-app-v2ray](https://github.com/rp-hello/luci-app-v2ray)

We keep package naming, struct same with [OpenWrt Official](https://github.com/openwrt/packages/tree/openwrt-22.03/net/v2ray-core).

## Install via OPKG

1. Download ipk files from [Latest Release](https://github.com/rp-hello/openwrt-v2ray/releases/latest).

2. install via opkg:

```sh
opkg install v2ray-*.ipk
# or
opkg install v2ray-core*.ipk v2ray-geoip*.ipk v2ray-geosite*.ipk
```

Bin file will install on `/usr/bin/v2ray`, asset_location will be `/usr/share/v2ray`.

## Custom build

Please take a look [build-openwrt.yml](./.github/workflows/build-openwrt.yml)

## Uninstall

```sh
opkg remove v2ray-core v2ray-geoip v2ray-geosite
```
