# 山月记

自然地理学背诵与间隔复习 Android 应用。当前提供 **0.3.2 本地学习测试版**，适配 Android 8.0 及以上。

## 下载与安装

- [直接下载安卓安装包](https://github.com/cymarlboro/shanyueji/releases/download/v0.3.2/shanyueji-0.3.2-3.apk)
- [版本说明与附件](https://github.com/cymarlboro/shanyueji/releases/tag/v0.3.2)

手机打开 APK，按系统提示安装。同签名新版直接覆盖安装，请勿先卸载，以保留本机资料与学习记录。

APK SHA-256：`5c7a1064749d3f2ae448af21652fbea3e125f2c21b299622f5068487f8c15c85`。

## 基础题库

安装包已内置 208 道题，首次使用不需要另外导入。仓库同时提供可单独查看、校验的数据：

- [基础题库 JSON](base-question-bank.json)：208 题、8 类题型、188 条生成答案草稿及出处。
- [读图题配图 JSON](base-question-images.json)：23 道读图题，共 26 张内嵌图片。
- [题库格式与复核说明](QUESTION_BANK.md)。

生成答案保留草稿与待复核标记，以 2024 版教材与原始来源核对，不代表全部审定。个人答案修订与学习记录不在公开题库中。

## 当前功能

复习支持显示答案、编辑保存、熟记与遗忘、自评后的间隔复习；题目可按章节、题干和题型筛选。支持本地资料解析、用户自配兼容 AI API、问答草稿确认与本地备份。

Supabase 私有数据库已经建立，但 **本版尚未接通云端账号登录、文件上传和管理员审核后台**。学习记录与用户资料仍以本机为准。

## 更新与隐私

后续版本统一在本仓库 Releases 发布。应用“我的 → 版本与更新”可填写更新清单地址：

`https://raw.githubusercontent.com/cymarlboro/shanyueji/main/update.json`

公开仓库不保存用户上传文件、个人记录、模型 API 密钥、数据库管理员凭据或应用签名私钥。请勿在公开 Issue 中提交密钥或私人资料。

基础资料原有版权归各权利人；本仓库不授予第三方教材、题目与图像的开源许可。
