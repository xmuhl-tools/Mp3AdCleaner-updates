# Mp3AdCleaner

更新发布通道：更新清单 + Windows x64 下载包（Mp3AdCleaner）。

- 当前版本：**1.1.0**（build 13）
- 最近更新：新增：无缝拼接广告检测（静音缝+头尾区间规则，覆盖整集重编码、无分隔字节的头尾广告，默认自动处理，可在设置或 config.ini 关闭）；新增：手动标记广告区间（右键菜单，时间区间吸附安全切点，可一键去广告或创建模板）；修复：中文文件名下创建模板名称为空；修复：手动标记对话框说明文字被裁/被遮挡；修复：AutoDeleteOnlyOnSafeBoundary 开关此前无效；UI 文本自适应门禁扩展多行高度与控件重叠维度；接受边界：静音缝启发式对合法长停顿有误报面（源只读、输出独立目录、可关闭）

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [Mp3AdCleaner-1.1.0.13-win-x64-Setup.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0/Mp3AdCleaner-1.1.0.13-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0/Mp3AdCleaner-1.1.0-win-x64.exe) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\Mp3AdCleaner`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0-win-x64.exe
  e25d5024d3b778c5a13dd0e6bff02afc7f67651abbdf5b2e821950ac3ee86d9a
Mp3AdCleaner-1.1.0.13-win-x64-Setup.exe
  ab7d890fdb7d23da6fb509be2fa647c32265ba839fe71015669d384dad4d71a7
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-17），请勿手工改动。
