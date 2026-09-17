# Mp3AdCleaner

更新发布通道：更新清单 + Windows x64 下载包（Mp3AdCleaner）。

- 当前版本：**1.1.0.14**（build 14）
- 最近更新：新增：无缝拼接广告检测扩展（短缝+电平差双向判据+逐段向后扩展），修复《解读希特勒》系列尾部安静广告漏检；修复：短缝候选在无长缝文件上不生效、内部停顿截断、日志电平符号；更新方案升级：RSA-2048 清单签名+客户端 fail-closed 验签；安装包改用 Inno Setup（带卸载入口，沿旧默认目录原地升级）；已知边界：静音缝启发式对安静收尾误报由 20s 下限防护

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [Mp3AdCleaner-1.1.0.14-win-x64-Setup.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.14/Mp3AdCleaner-1.1.0.14-win-x64-Setup.exe) |
| 便携版 / 自动更新载荷 | [Mp3AdCleaner-1.1.0.14-win-x64.exe](https://github.com/xmuhl-tools/Mp3AdCleaner-updates/releases/download/v1.1.0.14/Mp3AdCleaner-1.1.0.14-win-x64.exe) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\Mp3AdCleaner`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
Mp3AdCleaner-1.1.0.14-win-x64.exe
  185f90d6ccf626bfe0165cd3365a6eb4767b0ad4869e27e24082ca8caf0b5638
Mp3AdCleaner-1.1.0.14-win-x64-Setup.exe
  59baf4fbf75e0a0a01e2750d0d9fd7f5ae9fd3dc9644493636327bf272f64345
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-18），请勿手工改动。
