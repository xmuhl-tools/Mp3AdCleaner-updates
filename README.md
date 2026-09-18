# Mp3AdCleaner

更新发布通道：更新清单 + Windows x64 下载包（Mp3AdCleaner）。

- 当前版本：**1.1.0.15**（build 15）
- 最近更新：修复：界面与属性页版本号显示为完整版本（v1.1.0.15，含构建号）；沿袭 build 14 全部修复（短缝尾部检测双向判据、签名验签、Inno 安装包）

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [Mp3AdCleaner-1.1.0.15-win-x64-Setup.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.15/Mp3AdCleaner-1.1.0.15-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0.15-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.15/Mp3AdCleaner-1.1.0.15-win-x64.exe) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\Mp3AdCleaner`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0.15-win-x64.exe
  0fe90049184909c281a939a4376797e1debfa4a0fb85d4f479192691f0a89912
Mp3AdCleaner-1.1.0.15-win-x64-Setup.exe
  a977901a3c57559cc0560376a341bf9bae7c3de18fc953d0ba458a7f396a6979
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-18），请勿手工改动。
