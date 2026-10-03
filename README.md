# SwiftSign

SwiftSign 是一款 iOS 应用签名与管理工具，基于开源引擎 [Feather](https://github.com/khcrysalis/Feather) 构建，通过 GitHub Actions 云端打包（Cloud Build / 云打包）。

## 重要说明

> iOS 系统不允许未签名的应用直接安装。SwiftSign 云端打包产出的 `.ipa` 为**未签名**状态，需要用你的 Apple 证书（P12 + 描述文件）签名后才能安装。
> 装好 SwiftSign 之后，你可以在应用内导入 `.ipa` 和证书，软件会自动签名并安装——这正是选证书→自动签名的机制。

## 云打包

在 Actions 页签点击 `Cloud Build` 的 **Run workflow** 即可触发云端编译，产物（未签名 IPA）会出现在 Artifacts，打 tag（如 `v1.0.0`）时自动创建 Release 并附上 IPA。

## 官网

网站源码在仓库内，GitHub Pages 部署后即可访问。
