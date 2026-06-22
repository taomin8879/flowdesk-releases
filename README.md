# FlowDesk Releases

这个仓库只用于公开托管 FlowDesk 安装包、Tauri 自动更新文件和用户反馈。

不包含 FlowDesk 主程序闭源源码。

## 最新下载

```text
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/FlowDesk_V0_macOS-arm64.dmg
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/FlowDesk_V0_macOS-Intel.dmg
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/FlowDesk_V0_windows-x64.zip
```

## 自动更新

FlowDesk 应用内更新读取：

```text
https://github.com/taomin8879/flowdesk-releases/releases/latest/download/latest.json
```

V0 正式版先提供手动下载安装包。后续启用应用内自动更新时，需要将桌面端 `tauri.conf.json` 中的 updater endpoint 改成上述地址，并重新生成 Tauri updater artifacts、签名和 `latest.json`。

## 反馈

- 公开 bug / 功能建议：使用本仓库 Issues
- 私密反馈 / 购买 / 退款：tommy_ai@126.com

## 发布资产

每个 Release 至少包含：

- macOS Apple Silicon dmg
- macOS Intel dmg
- Windows x64 zip 或 installer
- `checksums.txt`

启用应用内自动更新后，还需要包含 Tauri updater artifacts、updater signature files 和 `latest.json`。

本模板中的 `releases/v0/` 目录已经放入当前三个公开安装包，方便你创建 GitHub Release 时直接上传。正式仓库可以只保留说明文件和 Issues，安装包主要放在 GitHub Release assets 里。

## 版本口径

当前公开版本：`v0` / `V0 正式版`

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
