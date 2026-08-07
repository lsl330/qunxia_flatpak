# 群侠集结 · Flatpak 打包仓库 (`qunxia_flatpak`)

> **Dream Jianghu** — Flathub 打包仓库，以**闭源 / 预编译**方式分发游戏启动器。
> App ID：`net.de5.qunxia.dream` · 支持架构：`x86_64` + `aarch64` · Runtime：`org.freedesktop.Platform 25.08`

---

## ⚠️ 关于「闭源」的重要说明

本仓库**只包含 Flathub 清单、元数据**，**不包含游戏二进制本身**。

游戏运行文件（启动器、3 个运行时 dylib、SDL3 动态库、字体）以**预编译**形式托管在

```
https://qunxia.de5.net/releases/
```

> 本仓库是**纯打包工程**；游戏源码与资产不在此仓库。



## English Abstract

This repository packages **Dream Jianghu** (群侠集结), a wuxia-themed RPG game launcher,
for **Flathub** as a **closed-source / precompiled** application.

- **App ID:** `net.de5.qunxia.dream`
- **Arches:** `x86_64` + `aarch64`
- **Runtime:** `org.freedesktop.Platform 25.08`

It contains **only** the Flathub manifest (`net.de5.qunxia.dream.yml`),
metadata (`*.desktop`, `*.metainfo.xml`, `icon.svg`), and the build scripts.
The actual game binaries are **not** stored here — they are precompiled and hosted at
`https://qunxia.de5.net/releases/`, downloaded at install time via `extra-data`
with sha256 verification.
