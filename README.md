# 山月记

自然地理学背诵与间隔复习软件，提供 Android 和 Windows x64 版本。当前待发布版本为 **0.4.0**。

## 下载与更新

- [Android 安装包](https://github.com/cymarlboro/shanyueji/releases/download/v0.4.0/shanyueji-0.4.0-4.apk)
- [Windows x64 安装包](https://github.com/cymarlboro/shanyueji/releases/download/v0.4.0/shanyueji-0.4.0-windows-x64-setup.exe)
- [版本说明与全部附件](https://github.com/cymarlboro/shanyueji/releases/tag/v0.4.0)
- [对应版本源码](https://github.com/cymarlboro/shanyueji/releases/download/v0.4.0/shanyueji-0.4.0-source.zip)
- [SHA256 校验清单](SHA256SUMS.txt)

安卓适配 Android 8.0 及以上。新版通过本仓库 Releases 发布，应用会检查官方更新清单并提示更新；安卓安装仍需系统确认。请直接覆盖安装，勿先卸载，以保留学习记录和配置。Windows 安装器暂未申请 Authenticode 证书。

## 学习与跨设备同步

内置 208 道题，覆盖 8 类题型。支持章节、题干和题型筛选、显示答案、编辑保存、熟记/遗忘、自评后的间隔复习，以及本地资料导入、兼容 AI API 解析、问答草稿确认和本地备份。

Android 与 Windows 可登录同一个云端账号。用户主动开启同步后，共享学习历史、答案修订、复习进度和已解析导入资料。登录本身不会自动上传；仍可离线学习。切换账号前请导出备份，并按应用中的绑定提示处理。

用户 API Key、密码和登录令牌不进入同步资料；普通用户看不到其他用户的资料。授权管理员可以审核上传的解析内容。公开仓库不保存用户上传文件、个人记录、数据库管理员凭据或应用签名私钥。请勿在公开 Issue 提交密钥或私人资料。

安卓准时提醒需要通知与精确闹钟授权，厂商后台策略仍可能影响送达。Windows 提醒需保持应用运行；休眠和系统通知设置也会影响送达。

## 基础题库

- [基础题库 JSON](base-question-bank.json)：208 题、8 类题型、188 条生成答案草稿及出处。
- [读图题配图 JSON](base-question-images.json)：23 道读图题，共 26 张图片。
- [题库格式与复核说明](QUESTION_BANK.md)。

答案生成稿以 2024 版教材与原始来源核对，用户可自行修订，不代表全部已审定。个人修订不进入公开基础题库。

## 开发与验证

版本源码附件包含 Android Java、Electron 桌面端、共享界面、数据库脚本及测试。Windows 更新清单使用 Ed25519 签名和安装包 SHA256 校验；安卓更新验证 APK 原应用签名。应用更新清单为：

https://raw.githubusercontent.com/cymarlboro/shanyueji/main/update.json

0.4.0 已通过本地两端回归、模拟器跨端资料测试、桌面正式打包内容启动/重启测试，以及真实 Supabase 事务内的账号隔离与 CAS 验证。尚未使用真实用户账号完成两台设备的联机同步验收。

基础资料原有版权归各权利人；本仓库不授予第三方教材、题目和图像的开源许可。
