# Mp3AdCleaner

更新发布通道：更新清单 + Windows x64 下载包（Mp3AdCleaner）。

- 当前版本：**1.1.0.20**（build 20）
- 最近更新：新增中部广告检测：整集重编码文件中部的无缝拼接广告（如《解读希特勒》系列 3 分 13 秒残留广告）现可自动识别为候选；默认转人工复核确认后完整无损切除，确认无误后可在 Config 配置开启自动处理

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [Mp3AdCleaner-1.1.0.20-win-x64-Setup.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.20/Mp3AdCleaner-1.1.0.20-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0.20-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.20/Mp3AdCleaner-1.1.0.20-win-x64.exe) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\Mp3AdCleaner`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0.20-win-x64.exe
  8843873274296be212d2c39ce4e63379611de6951c44c48c7e0023710abd9896
Mp3AdCleaner-1.1.0.20-win-x64-Setup.exe
  66c95f9e9fe773d7e45784b16cd689f8e2b56297236006ec7087ad2bb4088be1
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-10-05），请勿手工改动。
