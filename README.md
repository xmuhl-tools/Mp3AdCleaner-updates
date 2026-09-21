# Mp3AdCleaner

更新发布通道：更新清单 + Windows x64 下载包（Mp3AdCleaner）。

- 当前版本：**1.1.0.19**（build 19）
- 最近更新：修复检查更新在系统代理环境下的 send failed 失败：自动走系统代理、失败自动切换直连重试，失败原因记入日志文件

## 下载

| 用途 | 文件 |
|---|---|
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0.19-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.19/Mp3AdCleaner-1.1.0.19-win-x64.exe) |

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0.19-win-x64.exe
  8c114ac46f2b0c23fcbbd7701f23c9b94eb7161adfcf4e3e35f98a4b208399ca
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。
