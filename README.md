# LINE 移动端子设备协议方案 / LINE Mobile Sub-Device Protocol Solution

Chrome 插件版 LINE 计划在 `2026 年上半年` 下架，仍依赖网页版在线能力的业务，建议尽早准备切换方案。  
The LINE Chrome extension version is scheduled to be discontinued in `H1 2026`. If your business still depends on the web extension staying online, it is better to prepare a migration plan early.

这是一套基于 `LINE 移动端子设备` 的协议方案，可与主设备同时在线，适合作为 Chrome 插件版下架后的替代接入方案。  
This is a protocol solution based on `LINE mobile sub-devices`, capable of staying online together with the primary device, making it a practical replacement after the Chrome extension version is discontinued.

也可以理解为一套面向私有化部署场景的 `line api` / `line protocol` 方案，覆盖 `line ios`、`line ipad`、`line android` 等相关接入方向。  
It can also be understood as a private-deployment-oriented `line api` / `line protocol` solution covering `line ios`, `line ipad`, `line android`, and related integration scenarios.

## 相关关键词 / Keywords

- `LINE api` / LINE 接口方案
- `LINE protocol` / LINE 协议方案
- `LINE ios` / LINE iOS 接入
- `LINE ipad` / LINE iPad 接入
- `LINE android` / LINE Android 接入
- `LINE 移动端子设备协议` / LINE mobile sub-device protocol
- `LINE Chrome 插件替代方案` / LINE Chrome extension replacement
- `LINE 私有化部署协议` / LINE private deployment protocol
- `LINE 多账号托管方案` / LINE multi-account hosting solution
- `LINE 消息同步协议` / LINE message sync protocol

## 方案优势 / Advantages

- 资源消耗极低，适合托管大量账号 / Very low resource usage, suitable for hosting large numbers of accounts
- 基于纯协议算法实现，理解更深入，结构更清晰，便于持续维护与更新 / Built on pure protocol-level algorithm implementation, with deeper understanding, clearer structure, and easier long-term maintenance and updates
- 支持按业务需求定制功能 / Custom features can be developed for specific business needs
- 支持包月租用、私有化部署与源码交付 / Available as monthly rental, private deployment, or source code delivery

## 功能列表 / Features

### 登录与设备管理 / Login & Device Management

- 创建设备、查询设备详情 / Create devices and query device details
- 绑定回调地址、配置代理 / Bind callback URLs and configure proxies
- 子设备扫码登录、登录状态查询 / QR-based sub-device login and login status queries
- 在线状态维护 / Online session maintenance

### 消息能力 / Messaging

- 文本、图片、视频、音频、文件、贴图、名片发送 / Send text, image, video, audio, file, sticker, and contact card messages
- 消息撤回 / Unsend messages
- 已读同步、聊天移除状态同步 / Read sync and chat removed state sync

### 消息同步与回调 / Sync & Webhooks

- 消息盒子获取、会话列表分页 / Message box retrieval and paginated conversation listing
- 增量同步、历史消息获取 / Incremental sync and historical message retrieval
- 媒体下载 / Media download
- 新消息、已读、撤回、聊天变更、登录状态回调 / Webhook callbacks for new messages, reads, revokes, chat changes, and login status

### 联系人模块 / Contacts

- 好友 ID、联系人资料、目标资料、好友详情获取 / Retrieve friend IDs, contact profiles, target profiles, and detailed friend info
- 通过 MID 添加好友、删除好友 / Add friends by MID and delete friends
- 拉黑 / 取消拉黑、收藏状态、隐藏状态管理 / Block and unblock users, manage favorite status, and manage hidden status
- 好友备注名修改 / Update friend aliases
- 拉黑列表、推荐用户、好友请求、最近好友请求获取 / Retrieve block lists, recommended users, friend requests, and recent friend requests
- LINE 联系地址 / 二维码 ticket 获取与生成 / Get and generate LINE contact tickets / QR tickets
- 通过 searchId 或 ticket 查找联系人 / Find contacts by searchId or ticket
- 个人资料更新、用户主页资料获取 / Update profile info and fetch home profile data

### 群聊与会话模块 / Chats & Sessions

- 全部聊天列表、聊天详情批量获取 / Retrieve all chat IDs and batch chat details
- 创建群聊、更新聊天信息 / Create chats and update chat info
- 邀请成员入群、移除群成员、主动退群 / Invite members, remove members, and leave chats
- 聊天通知设置获取与更新 / Get and update chat notification settings
- 聊天隐藏状态设置 / Set chat hidden status
- 账号资料获取、会话配置获取、会话登出 / Get account profile, fetch session configurations, and logout sessions

### 贴图商店与扩展能力 / Sticker Store & Extended Capabilities

- 贴图商店详情获取 / Get sticker store item details
- 贴图商店最新版本获取 / Get latest sticker store versions
- 已拥有贴图列表获取 / Get owned sticker lists
- 频道信息与频道令牌相关能力 / Channel info and channel token related capabilities
- E2EE 公钥、群组密钥相关能力 / E2EE public key and group key related capabilities

## 交付方式 / Delivery Options

### 包月租用 / Monthly Rental

- `50 $ / 号 / 月` / `50 USD / account / month`

### 私有化部署 / Private Deployment

- `5000 $` / `5000 USD`
- 二进制交付 / Binary delivery
- 每次更新 `+500 $` / `+500 USD per update`

### 源码购买 / Source Code Purchase

- `10000 $` / `10000 USD`
- 架构清晰 / Clear architecture
- 有技术团队可自行维护 / Teams with engineering capability can maintain it independently

### 免费试用 / Free Trial

- 提供测试环境 / Test environment available
- 服务器配置较低，稳定性一般 / Trial server has low specs and limited stability
- 仅供功能验证，不建议正式业务使用 / For feature verification only, not recommended for production use
- TG 联系获取试用地址 / Contact on Telegram for the trial address: [https://t.me/Gareth9527](https://t.me/Gareth9527)

## 一句话介绍 / One-Line Summary

> 这是一套基于 LINE 移动端子设备的协议方案，可与主设备同时在线，资源占用低、可托管大量账号，适合在 Chrome 插件版于 2026 年上半年停止服务前，提前完成业务切换。  
> This is a LINE mobile sub-device protocol solution that can stay online together with the primary device, uses very little system resource, supports large-scale account hosting, and is suitable for completing migration before the Chrome extension version is discontinued in H1 2026.
