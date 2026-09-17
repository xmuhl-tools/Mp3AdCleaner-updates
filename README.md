# Mp3AdCleaner

MP3 批量无损去广告工具：自动识别并无损删除 MP3 中的插入广告（正文不重编码），Windows x64 绿色工具。

- 当前版本：**1.1.0**（build 12）
- 最近更新：修复：状态栏提示文字截断；修复：最大化后还原日志框消失；修复：设置对话框标签与复选框重叠；新增对话框布局守卫（文字宽度+控件重叠双维度）；发布渠道迁移到组织仓库 xmuhl-tools/Mp3AdCleaner-updates；提供免注册表安装包

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [Mp3AdCleaner-1.1.0.12-win-x64-Setup.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0/Mp3AdCleaner-1.1.0.12-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0/Mp3AdCleaner-1.1.0-win-x64.exe) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%/Mp3AdCleaner`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0-win-x64.exe
  397e4408fb95d8ac7a127b3af21c1ed75af91a806e1d52d2c325fc90772ea4b6
Mp3AdCleaner-1.1.0.12-win-x64-Setup.exe
  abe6b9b6162418125a9ed006919bee9d781b7f40ac8851ff9d19e23d13ed946e
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-17），请勿手工改动。
