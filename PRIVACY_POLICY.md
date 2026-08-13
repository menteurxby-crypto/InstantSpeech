# 隐私政策 / Privacy Policy

> **最后更新 / Last updated:** 2026 年 8 月 13 日 / August 13, 2026
> **开发者 / Developer:** 徐博宇
> **联系邮箱 / Contact:** 183835370@qq.com
> **托管地址 / Hosted at:** {{隐私政策托管 URL}}（GitHub Pages 部署后填入）

---

## 一、中文版

**瞬言（InstantSpeech）**（以下简称"本应用"）是一款帮助用户提升口头表达能力的工具应用。我们深知您的隐私和数据安全的重要性，特制定本隐私政策，说明我们如何处理您的信息。

### 1. 我们收集的信息

| 数据类型 | 说明 | 存储位置 |
|---|---|---|
| **录音音频** | 仅当您主动点击录音时采集，用于语音转写与分析 | 仅存储在您的设备本地；已排除 iCloud 备份 |
| **转写文本** | 由录音音频识别生成的文字内容 | 设备本地 + 通过 iCloud（CloudKit）在您的设备间同步 |
| **统计指标** | 语速、停顿、填充词、词汇丰富度等由本地计算的分析数据 | 设备本地 + iCloud 同步 |
| **AI 分析文本** | 您主动请求"AI 教练"时，转写文本会发送至我们自建的服务器，用于内容层面的表达分析 | 仅在传输与处理过程中短暂存在，服务器端不存储 |
| **订阅信息** | 您购买订阅服务时的交易信息（由 Apple 处理） | Apple（App Store / StoreKit） |
| **匿名标识符** | 用于 API 限流与数据隔离的随机 user_id | 设备本地 |

**我们不会收集**：您的姓名、手机号、通讯录、位置信息、照片等与核心功能无关的个人信息。

### 2. 我们如何使用信息

- 提供核心功能：录音转写、表达统计、AI 教练反馈
- 同步您的数据：通过 iCloud（CloudKit）在您本人的设备间同步转写与分析数据
- 保护服务安全：对 AI 分析接口按 user_id 限流，防止滥用
- **我们不会**将您的数据用于广告投放、出售给第三方或用于任何与产品无关的目的

### 3. AI 教练的数据处理说明

当您使用"AI 教练"功能时：

1. 仅有**转写文本**（非音频）会被发送至我们自建的代理服务器（位于中国境内腾讯云服务器）；
2. 代理服务器将文本转发给第三方 AI 服务提供商（DeepSeek，深度求索公司）进行内容分析；
3. 所有传输均通过 **HTTPS 加密**；
4. 代理服务器**不存储**您的文本内容，仅做实时转发与限流；
5. 分析结果返回后保存在您的设备与 iCloud 账户内。

**您的数据不会出境**：录音、文本与 AI 分析的处理均发生在中国大陆境内。

### 4. 信息共享与第三方

- **Apple**：iCloud（CloudKit）同步、App Store 订阅与支付由 Apple 处理，我们无法访问您的支付信息
- **DeepSeek（深度求索）**：接收您主动请求的 AI 分析文本，仅用于生成表达反馈
- **腾讯云**：托管自建代理服务器（数据在传输过程中经过）

除上述为实现核心功能所必需的第三方外，我们不会向任何第三方出售、出租或共享您的个人信息。

### 5. 数据安全

- 录音音频仅存于设备本地，并排除 iCloud 备份（音频不会上传到任何服务器）
- 网络传输全程 HTTPS 加密
- AI 接口采用按用户限流 + 请求体大小限制，API 密钥仅保存在服务器端
- 我们采取合理的技术与管理措施保护数据安全

### 6. 您的权利

- **访问与更正**：您可以在应用内随时查看您的转写记录与分析报告
- **删除**：您可以在应用内随时删除任意录音、转写记录及其分析报告；删除后数据将被移除（iCloud 同步副本也将删除）
- **停止使用**：卸载应用并删除所有记录即停止数据处理
- **撤回授权**：您可随时在系统设置中关闭麦克风权限

### 7. 数据保留

- 录音与转写数据保留在您的设备与 iCloud 账户内，直到您主动删除
- AI 分析文本在服务器端不存储，处理完成后即释放

### 8. 儿童隐私

本应用不面向 13 周岁以下儿童，我们不会有意收集儿童的个人信息。如您认为我们无意中收集了儿童信息，请联系我们删除。

### 9. 政策变更

我们可能不时更新本隐私政策。重大变更将在应用内显著位置通知您。更新后的政策将在本页面发布并注明更新日期。

### 10. 联系我们

如您对本隐私政策有任何疑问或请求，请通过以下方式联系我们：

- 邮箱：183835370@qq.com
- 生效日期：2026 年 8 月 13 日

---

## 2. English Version

**InstantSpeech** (the "App") is a tool that helps users improve their oral expression skills. We take your privacy and data security seriously. This Privacy Policy explains how we handle your information.

### 2.1 Information We Collect

| Data Type | Description | Storage |
|---|---|---|
| **Audio Recordings** | Captured only when you actively start a recording, used for speech transcription and analysis | Stored locally on your device only; excluded from iCloud backup |
| **Transcription Text** | Text generated from your audio recordings via speech recognition | On your device + synced across your devices via iCloud (CloudKit) |
| **Analytics Metrics** | Locally computed metrics such as speech rate, pauses, filler words, and vocabulary richness | On your device + synced via iCloud |
| **AI Analysis Text** | When you actively request the "AI Coach", your transcription text is sent to our self-hosted server for content-level expression analysis | Exists only transiently during transmission and processing; not stored on the server |
| **Subscription Information** | Transaction details when you purchase a subscription (processed by Apple) | Apple (App Store / StoreKit) |
| **Anonymous Identifier** | A random user_id used for API rate limiting and data isolation | On your device |

**We do NOT collect**: your name, phone number, contacts, location, photos, or any personal information unrelated to the core functionality.

### 2.2 How We Use Your Information

- To provide core functionality: recording transcription, expression analytics, and AI coach feedback
- To sync your data: via iCloud (CloudKit) across your own devices
- To protect our service: rate limiting the AI analysis endpoint by user_id to prevent abuse
- **We will NOT** use your data for advertising, sell it to third parties, or use it for any purpose unrelated to the product

### 2.3 AI Coach Data Processing

When you use the "AI Coach" feature:

1. Only the **transcription text** (not audio) is sent to our self-hosted proxy server (hosted on Tencent Cloud, mainland China);
2. The proxy forwards the text to a third-party AI provider (DeepSeek) for content analysis;
3. All transmission is protected by **HTTPS encryption**;
4. The proxy **does not store** your text — it only forwards in real time and enforces rate limits;
5. Analysis results are stored on your device and in your iCloud account.

**Your data does not leave mainland China**: audio, text, and AI analysis processing all occur within mainland China.

### 2.4 Information Sharing and Third Parties

- **Apple**: iCloud (CloudKit) sync, App Store subscriptions, and payments are processed by Apple. We never access your payment information
- **DeepSeek**: Receives the AI analysis text you actively request, used solely to generate expression feedback
- **Tencent Cloud**: Hosts our self-hosted proxy server (data passes through during transmission)

Apart from the above parties that are strictly necessary to provide core functionality, we do not sell, rent, or share your personal information with any third party.

### 2.5 Data Security

- Audio recordings are stored locally only and excluded from iCloud backup (audio is never uploaded to any server)
- All network transmission is encrypted with HTTPS
- The AI endpoint enforces per-user rate limiting and payload size limits; the API key is stored on the server side only
- We take reasonable technical and administrative measures to protect your data

### 2.6 Your Rights

- **Access and correction**: You can view your transcription records and analysis reports anytime within the App
- **Deletion**: You can delete any recording, transcription record, and its analysis report anytime within the App; deleted data will be removed (including iCloud synced copies)
- **Stop using**: Uninstalling the App and deleting all records stops data processing
- **Withdraw consent**: You can revoke microphone access anytime in your system settings

### 2.7 Data Retention

- Recordings and transcription data remain on your device and in your iCloud account until you delete them
- AI analysis text is not stored on the server; it is released as soon as processing completes

### 2.8 Children's Privacy

The App is not intended for children under 13, and we do not knowingly collect personal information from children. If you believe we have unintentionally collected a child's information, please contact us for deletion.

### 2.9 Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be notified prominently within the App. The updated policy will be published on this page with the revised date.

### 2.10 Contact Us

If you have any questions or requests regarding this Privacy Policy, please contact us at:

- Email: 183835370@qq.com
- Effective date: August 13, 2026
