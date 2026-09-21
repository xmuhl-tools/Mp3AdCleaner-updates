# Mp3AdCleaner

更新发布通道：更新清单 + Windows x64 下载包（Mp3AdCleaner）。

- 当前版本：**1.1.0.18**（build 18）
- 最近更新：修复自动更新下载偶发挂死（portable-app-release 模板家族性缺陷）：下载读循环新增停滞中止保护——任一下载源 15 秒无字节进展即放弃并换下一源（原实现仅依赖 WinHTTP 逐操作超时，代理"涓流"喂字节时可无限挂死，界面永远停在下载中）；程序功能本身无变化。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [Mp3AdCleaner-1.1.0.18-win-x64-Setup.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.18/Mp3AdCleaner-1.1.0.18-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0.18-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.18/Mp3AdCleaner-1.1.0.18-win-x64.exe) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\Mp3AdCleaner`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0.18-win-x64.exe
  6f96a7dc0b496a33b053706713dc1a4f87f28def467177802bb0e4b63602d3aa
Mp3AdCleaner-1.1.0.18-win-x64-Setup.exe
  1af0521e4c6148ef86ddd4bba3f61c5b3336a9d4e2ba7b5961f1cffe535a9b0b
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-21），请勿手工改动。
