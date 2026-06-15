# FlowDesk 发版清单

## 发布前

- [ ] 确认版本号，例如 `0.5.6-beta`
- [ ] 更新 FlowDesk 桌面端 `package.json`
- [ ] 更新 `src-tauri/tauri.conf.json`
- [ ] 确认 updater endpoint 为 `https://github.com/taomin8879/flowdesk-releases/releases/latest/download/latest.json`
- [ ] 更新官网 changelog
- [ ] 本地跑核心测试
- [ ] 构建 macOS Apple Silicon
- [ ] 构建 macOS Intel
- [ ] 构建 Windows x64
- [ ] 生成 updater artifacts
- [ ] 生成 signature
- [ ] 生成 SHA256

## 发布 GitHub Release

- [ ] 创建 tag，例如 `v0.5.6-beta`
- [ ] 上传用户安装包
- [ ] 上传 updater artifacts
- [ ] 上传 `.sig` 文件
- [ ] 上传 `latest.json`
- [ ] 上传 `checksums.txt`
- [ ] Release notes 写明更新内容、已知问题和系统要求

## 发布后验证

- [ ] 官网下载按钮可下载三个平台安装包
- [ ] `checksums.txt` 与安装包一致
- [ ] 老版本点击检查更新能看到新版本
- [ ] 更新包签名验证通过
- [ ] GitHub Issues 可提交反馈
- [ ] 邮箱购买流程文案仍然正确
