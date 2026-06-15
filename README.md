# FlowDesk Releases

这个仓库只用于公开托管 FlowDesk 安装包、Tauri 自动更新文件和用户反馈。

不包含 FlowDesk 主程序闭源源码。

## 最新下载

```text
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/FlowDesk_0.5.5-beta_macOS-arm64.dmg
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/FlowDesk_0.5.5-beta_macOS-Intel.dmg
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/FlowDesk_0.5.5-beta_windows-x64.zip
```

## 自动更新

FlowDesk 应用内更新读取：

```text
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/latest.json
```

正式发布前，需要将桌面端 `tauri.conf.json` 中的 updater endpoint 改成上述地址，并重新构建安装包。

## 反馈

- 公开 bug / 功能建议：使用本仓库 Issues
- 私密反馈 / 购买 / 退款：tommy_ai@126.com

## 发布资产

每个 Release 至少包含：

- macOS Apple Silicon dmg
- macOS Intel dmg
- Windows x64 zip 或 installer
- Tauri updater artifacts
- updater signature files
- `latest.json`
- `checksums.txt`

本模板中的 `releases/v0.5.5-beta/` 目录已经放入当前三个公开安装包，方便你创建 GitHub Release 时直接上传。正式仓库可以只保留说明文件和 Issues，安装包主要放在 GitHub Release assets 里。

## 版本口径

当前建议公开版本：`v0.5.5-beta`

支持平台：

- macOS Apple Silicon
- macOS Intel
- Windows x64

不承诺：

- Linux
- Web
- iOS / Android
- 云同步
- 团队协作
