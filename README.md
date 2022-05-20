<p align="center">
    <a href="https://www.finclip.com?from=github">
    <img width="auto" src="https://www.finclip.com/mop/document/images/logo.png">
    </a>
</p>

<p align="center"> 
    <strong>FinClip 微信登录授权页面</strong></br>
<p>
<p align="center"> 
        本项目提供在小程序中复用微信登录的能力，用户可将对应资源上传至微信与 FinClip 小程序代码包中完成实现。
<p>

<p align="center"> 
	👉 <a href="https://www.finclip.com?from=github">https://www.finclip.com/</a> 👈
</p>

<div align="center">

<a href="#"><img src="https://img.shields.io/badge/%E4%B8%93%E5%B1%9E%E5%BC%80%E5%8F%91%E8%80%85-20000%2B-brightgreen"></a>
<a href="#"><img src="https://img.shields.io/badge/%E5%B7%B2%E4%B8%8A%E6%9E%B6%E5%B0%8F%E7%A8%8B%E5%BA%8F-6000%2B-blue"></a>
<a href="#"><img src="https://img.shields.io/badge/%E5%B7%B2%E9%9B%86%E6%88%90%E5%B0%8F%E7%A8%8B%E5%BA%8F%E5%BA%94%E7%94%A8-75%2B-yellow"></a>
<a href="#"><img src="https://img.shields.io/badge/%E5%AE%9E%E9%99%85%E8%A6%86%E7%9B%96%E7%94%A8%E6%88%B7-2500%20%E4%B8%87%2B-orange"></a>

<a href="https://www.zhihu.com/org/finchat"><img src="https://img.shields.io/badge/FinClip--lightgrey?logo=zhihu&style=social"></a>
<a href="https://www.finclip.com/blog/"><img src="https://img.shields.io/badge/FinClip%20Blog--lightgrey?logo=ghost&style=social"></a>



</div>

<p align="center">

<div align="center">

[官方网站](https://www.finclip.com/) | [示例小程序](https://www.finclip.com/#/market) | [开发文档](https://www.finclip.com/mop/document/) | [部署指南](https://www.finclip.com/mop/document/introduce/quickStart/cloud-server-deployment-guide.html) | [SDK 集成指南](https://www.finclip.com/mop/document/introduce/quickStart/intergration-guide.html) | [API 列表](https://www.finclip.com/mop/document/develop/api/overview.html) | [组件列表](https://www.finclip.com/mop/document/develop/component/overview.html) | [隐私承诺](https://www.finclip.com/mop/document/operate/safety.html)

</div>

-----
## 🤔 FinClip 是什么?

有没有**想过**，开发好的微信小程序能放在自己的 APP 里直接运行，只需要开发一次小程序，就能在不同的应用中打开它，是不是很不可思议？

有没有**试过**，在自己的 APP 中引入一个 SDK ，应用中不仅可以打开小程序，还能自定义小程序接口，修改小程序样式，是不是觉得更不可思议？

这就是 FinClip ，就是有这么多不可思议！

## ⚙️ 操作步骤
### 1. 微信登录功能与流程介绍
* FinClip 小程序调用接口（`wx.login`, `wx.getUserProfile`，`wx.getPhoneNumber`）
* App 端注入接口（`wx.login`, `wx.getUserProfile`，`wx.getPhoneNumber`）
* App端引入 wx 端 openSDK，获取管理后台配置的微信登录小程序相关信息
* 执行 `WXLaunchMiniProgram` 方法打开微信登录小程序的授权页面
* 小程序根据 App 的参数执行相关的微信接口获取信息，并返回 App
* App 把接口数据回传给凡泰小程序

### 2. 微信登录配置说明
* 准备一个微信登录小程序
* 从[这里](https://github.com/finogeeks/wechat-auth-page))获取授权页面
* 由于`wx.getPhoneNumber` Api需要服务端解密接口，所以需要自行修改这里的接口
* 前往微信公众平台上架微信登录小程序（也可集成在已有的微信小程序里）
* 前往 FinClip 管理后台【小程序管理-我的小程序-第三方管理】进行配置
* App 端实现相关的微信接口（`wx.login`, `wx.getUserProfile`，`wx.getPhoneNumber`)
* 上架相关小程序，进行调试

### 3. 登录流程
本微信登录功能采用了 [小程序登录常见问题](/faq/app/wechat-login-issue.html) 中的方案三，您需要在您已有微信小程序中进行定义修改，从而使得 FinClip 小程序具备微信登录的能力，具体流程图如下所示。

![image.png](https://raw.githubusercontent.com/finogeeks/wechat-auth-page/main/image.png)

## 📋 集成文档
[点击这里](https://www.finclip.com/mop/document/introduce/quickStart/intergration-guide.html#_1-ios-%E5%BF%AB%E9%80%9F%E9%9B%86%E6%88%90) 查看 iOS 快速集成文档

## 🔗 常用链接
以下内容是您在 FinClip 进行开发与体验时，常见的问题与指引信息

- [FinClip 官网](https://www.finclip.com/#/home)
- [示例小程序](https://www.finclip.com/#/market)
- [文档中心](https://www.finclip.com/mop/document/)
- [SDK 部署指南](https://www.finclip.com/mop/document/introduce/quickStart/intergration-guide.html)
- [小程序代码结构](https://www.finclip.com/mop/document/develop/guide/structure.html)
- [iOS 集成指引](https://www.finclip.com/mop/document/runtime-sdk/ios/ios-integrate.html)
- [Android 集成指引](https://www.finclip.com/mop/document/runtime-sdk/android/android-integrate.html)
- [Flutter 集成指引](https://www.finclip.com/mop/document/runtime-sdk/flutter/flutter-integrate.html)

## ☎️ 联系我们
微信扫描下面二维码，关注官方公众号 **「凡泰极客」**，获取更多精彩内容。<br>
<img width="150px" src="https://www.finclip.com/mop/document/images/ic_qr.svg">

微信扫描下面二维码，邀请进官方微信交流群（加好友备注：finclip 咨询），获取更多精彩内容。<br>
<img width="150px" src="https://finclip-homeweb-1251849568.cos.ap-guangzhou.myqcloud.com/images/ldy111.jpg">

## Stargazers
[![Stargazers repo roster for @finogeeks/finclip-ios-demo](https://reporoster.com/stars/finogeeks/wechat-auth-page)](https://github.com/finogeeks/wechat-auth-page/stargazers)

## Forkers
[![Forkers repo roster for @finogeeks/finclip-ios-demo](https://reporoster.com/forks/finogeeks/wechat-auth-page)](https://github.com/finogeeks/finclip-ios-demo/network/members)
