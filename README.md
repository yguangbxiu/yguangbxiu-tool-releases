# YguangbxiuTool 发布产物

本仓库只存放 YguangbxiuTool 的官方发布产物，**不包含源代码**。源码仓库保持私有。

## 下载

- 最新版本：<https://github.com/yguangbxiu/yguangbxiu-tool-releases/releases/latest>
- 自动更新源（应用内使用）：<https://github.com/yguangbxiu/yguangbxiu-tool-releases/releases/latest/download/appcast.xml>
- 历史发布记录：[CHANGELOG.md](CHANGELOG.md)

每个版本包含：

| 文件 | 用途 |
| --- | --- |
| `YguangbxiuTool-x.y.z.zip` | 应用本体 |
| `YguangbxiuTool-x.y.z.zip.sha256` | SHA-256 校验文件 |
| `appcast.xml` | Sparkle 更新源（0.2.0 起） |

## 安装与校验

1. 下载 zip 与同名 `.sha256`，在终端执行 `shasum -a 256 -c YguangbxiuTool-x.y.z.zip.sha256`。
2. 解压后把 `YguangbxiuTool.app` 拖进「应用程序」再运行。
3. 首次打开若提示"未识别的开发者"，在 Finder 中右键应用 → 打开，确认一次即可。

应用内的后续升级由 EdDSA 签名校验保证完整性；签名公钥内嵌在应用里，不依赖 Apple 公证。

## 关于 “Source code”

Release 页面上的 “Source code (zip/tar.gz)” 指向本仓库的占位提交，**不是应用源码**。本仓库没有源码历史。
