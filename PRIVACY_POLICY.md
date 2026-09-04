# 隐私政策 / Privacy Policy

> **最后更新 / Last updated:** 2026 年 9 月 4 日 / September 4, 2026
> **开发者 / Developer:** 徐博宇
> **联系邮箱 / Contact:** 183835370@qq.com
> **托管地址 / Hosted at:** https://menteurxby-crypto.github.io/InstantSpeech/PRIVACY_POLICY.html

---

## 一、中文版

**瞬言（InstantSpeech）**（以下简称"本应用"）是一款帮助用户提升口头表达能力的工具应用。我们深知您的隐私和数据安全的重要性，特制定本隐私政策，说明我们如何处理您的信息。

### 1. 我们收集的信息

| 数据类型 | 说明 | 存储位置 |
|---|---|---|
| **录音音频** | 仅当您主动点击录音时采集，用于语音转写与分析 | 本地存储，已排除 iCloud 备份；使用云端转写时按块经 HTTPS 上传至自建服务器（见第 3 节），服务器不留存音频 |
| **转写文本** | 由录音音频识别生成的文字内容（设备端识别与云端转写双轨） | 设备本地 + 通过 iCloud（CloudKit）在您的设备间同步 |
| **统计指标** | 语速、停顿、填充词、词汇丰富度等由本地计算的分析数据 | 设备本地 + iCloud 同步 |
| **AI 分析文本** | 您主动请求"AI 教练"时，转写文本会发送至我们自建的服务器，用于内容层面的表达分析 | 仅在传输与处理过程中短暂存在，服务器端不存储 |
| **AI 改写文本** | 您主动请求"全文改写"时，练习稿文本会发送至我们自建的服务器，用于生成改写建议 | 仅在传输与处理过程中短暂存在，服务器端不存储 |
| **订阅信息** | 您购买订阅服务时的交易信息（由 Apple 处理） | Apple（App Store / StoreKit） |
| **匿名标识符** | 用于 API 限流与数据隔离的随机 user_id | 设备本地 |
| **匿名使用数据（埋点）** | 功能使用事件（录音开始/完成/取消与时长、AI 分析与改写请求及结果、页面浏览、付费成功等），关联匿名 user_id，**不含音频与转写原文** | 自建服务器（api.life-log.top，腾讯云）+ 设备本地暂存 |

**我们不会收集**：您的姓名、手机号、通讯录、位置信息、照片等与核心功能无关的个人信息。

### 2. 我们如何使用信息

- 提供核心功能：录音转写、表达统计、AI 教练反馈与全文改写
- 同步您的数据：通过 iCloud（CloudKit）在您本人的设备间同步转写与分析数据
- 保护服务安全：对 AI 分析接口按 user_id 限流，防止滥用
- 产品改进与增长分析：基于匿名使用数据统计功能使用情况（录音时长、AI 分析成功率、页面使用频次等），不识别个人
- **我们不会**将您的数据用于广告投放、出售给第三方或用于任何与产品无关的目的

### 3. 云端转写与 AI 功能的数据处理说明

**云端语音转写**

1. 录音时，App 会同时使用设备端识别与云端转写（双轨并行，互为补充）；
2. 云端转写会将录音按块转换为 16kHz 单声道音频，经 **HTTPS 加密**上传至我们自建的转写接口（位于中国境内腾讯云服务器），仅用于生成文字；
3. 转写接口**不存储**音频，处理完成后即释放；云端服务不可用时自动仅使用设备端识别。

**AI 教练与 AI 全文改写**

当您主动使用"AI 教练"或"全文改写"功能时：

1. 仅有**文本**（转写文本或练习稿文本，非音频）会被发送至我们自建的代理服务器（位于中国境内腾讯云服务器）；
2. 代理服务器将文本按回退顺序转发给第三方 AI 服务提供商（商汤"日日新" SenseNova 与/或 DeepSeek，深度求索公司）进行表达分析或改写；
3. 所有传输均通过 **HTTPS 加密**；
4. 代理服务器**不存储**您的文本内容，仅做实时转发与限流；
5. 分析与改写结果返回后保存在您的设备与 iCloud 账户内。

**您的数据不会出境**：音频转写、文本与 AI 处理均发生在中国大陆境内。

### 4. 信息共享与第三方

- **Apple**：iCloud（CloudKit）同步、App Store 订阅与支付由 Apple 处理，我们无法访问您的支付信息
- **商汤科技（日日新 SenseNova）**：接收您主动请求的 AI 分析与改写文本（经自建代理转发），仅用于生成表达反馈与改写
- **DeepSeek（深度求索）**：同上，作为 AI 分析与改写的回退服务提供商
- **腾讯云**：托管自建代理与转写服务器（数据在传输过程中经过）

除上述为实现核心功能所必需的第三方外，我们不会向任何第三方出售、出租或共享您的个人信息。

### 5. 数据安全

- 录音音频存于设备本地并排除 iCloud 备份；云端转写时音频按块经 HTTPS 上传，仅用于实时转写、服务器不留存
- 网络传输全程 HTTPS 加密
- 云端转写与 AI 接口均采用按用户限流 + 请求体大小限制，API 密钥仅保存在服务器端
- 匿名使用数据（埋点）经 HTTPS 加密发送至自建服务器（与 AI 代理同域 api.life-log.top），仅含事件名与行为属性，不含音频与转写原文
- 我们采取合理的技术与管理措施保护数据安全

### 6. 您的权利

- **访问与更正**：您可以在应用内随时查看您的转写记录与分析报告
- **删除**：您可以在应用内随时删除任意录音、转写记录及其分析报告；删除后数据将被移除（iCloud 同步副本也将删除）
- **停止使用**：卸载应用并删除所有记录即停止数据处理
- **撤回授权**：您可随时在系统设置中关闭麦克风或语音识别权限；关闭后云端转写仍可独立使用（如需彻底停止云端上传，请勿使用录音功能或联系我们）

### 7. 数据保留

- 录音与转写数据保留在您的设备与 iCloud 账户内，直到您主动删除
- AI 分析与改写文本在服务器端不存储，处理完成后即释放

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
| **Audio Recordings** | Captured only when you actively start a recording, used for speech transcription and analysis | Stored locally, excluded from iCloud backup; when cloud transcription is used, audio chunks are uploaded over HTTPS to our self-hosted server (see Section 3) and not retained |
| **Transcription Text** | Text generated from your audio recordings (on-device recognition + cloud transcription, dual-track) | On your device + synced across your devices via iCloud (CloudKit) |
| **Analytics Metrics** | Locally computed metrics such as speech rate, pauses, filler words, and vocabulary richness | On your device + synced via iCloud |
| **AI Analysis Text** | When you actively request the "AI Coach", your transcription text is sent to our self-hosted server for content-level expression analysis | Exists only transiently during transmission and processing; not stored on the server |
| **AI Rewrite Text** | When you actively request "Full-Text Rewrite", your practice draft text is sent to our self-hosted server to generate rewrite suggestions | Exists only transiently during transmission and processing; not stored on the server |
| **Subscription Information** | Transaction details when you purchase a subscription (processed by Apple) | Apple (App Store / StoreKit) |
| **Anonymous Identifier** | A random user_id used for API rate limiting and data isolation | On your device |
| **Anonymous Usage Data (Analytics)** | Feature usage events (recording start/complete/cancel and duration, AI analysis and rewrite requests and outcomes, page views, purchase success, etc.), tied to the anonymous user_id. **Does not include audio or transcription text** | Self-hosted server (api.life-log.top, Tencent Cloud) + temporarily stored on device |

**We do NOT collect**: your name, phone number, contacts, location, photos, or any personal information unrelated to the core functionality.

### 2.2 How We Use Your Information

- To provide core functionality: recording transcription, expression analytics, AI coach feedback, and full-text rewrite
- To sync your data: via iCloud (CloudKit) across your own devices
- To protect our service: rate limiting the AI analysis endpoint by user_id to prevent abuse
- Product improvement and growth analytics: we aggregate anonymous usage data (recording duration, AI analysis success rate, feature usage frequency, etc.) to improve the product; this does not identify individuals
- **We will NOT** use your data for advertising, sell it to third parties, or use it for any purpose unrelated to the product

### 2.3 Cloud Transcription and AI Feature Data Processing

**Cloud speech transcription**

1. During recording, the App uses both on-device recognition and cloud transcription in parallel (dual-track, complementary);
2. Cloud transcription converts recording chunks into 16kHz mono audio and uploads them over **HTTPS** to our self-hosted transcription endpoint (hosted on Tencent Cloud, mainland China), solely to generate text;
3. The transcription endpoint **does not store** audio — it is released once processing completes; if the cloud service is unavailable, the App automatically falls back to on-device recognition only.

**AI Coach & Full-Text Rewrite**

When you actively use the "AI Coach" or "Full-Text Rewrite" feature:

1. Only **text** (transcription text or practice draft text, never audio) is sent to our self-hosted proxy server (hosted on Tencent Cloud, mainland China);
2. The proxy forwards the text, in fallback order, to third-party AI providers (SenseNova "RiRiXin" by SenseTime and/or DeepSeek) for expression analysis or rewriting;
3. All transmission is protected by **HTTPS encryption**;
4. The proxy **does not store** your text — it only forwards in real time and enforces rate limits;
5. Analysis and rewrite results are stored on your device and in your iCloud account.

**Your data does not leave mainland China**: audio transcription, text, and AI processing all occur within mainland China.

### 2.4 Information Sharing and Third Parties

- **Apple**: iCloud (CloudKit) sync, App Store subscriptions, and payments are processed by Apple. We never access your payment information
- **SenseTime (SenseNova)**: Receives the AI analysis and rewrite text you actively request (via our proxy), used solely to generate expression feedback and rewrites
- **DeepSeek**: Same as above, serving as the fallback provider for AI analysis and rewriting
- **Tencent Cloud**: Hosts our self-hosted proxy and transcription servers (data passes through during transmission)

Apart from the above parties that are strictly necessary to provide core functionality, we do not sell, rent, or share your personal information with any third party.

### 2.5 Data Security

- Audio recordings are stored locally and excluded from iCloud backup; during cloud transcription, audio chunks are uploaded over HTTPS solely for real-time transcription and are not retained
- All network transmission is encrypted with HTTPS
- Both the cloud transcription and AI endpoints enforce per-user rate limiting and payload size limits; API keys are stored on the server side only
- Anonymous usage data (analytics) is sent over HTTPS to our self-hosted server (api.life-log.top, same domain as the AI proxy), containing only event names and behavior attributes — never audio or transcription text
- We take reasonable technical and administrative measures to protect your data

### 2.6 Your Rights

- **Access and correction**: You can view your transcription records and analysis reports anytime within the App
- **Deletion**: You can delete any recording, transcription record, and its analysis report anytime within the App; deleted data will be removed (including iCloud synced copies)
- **Stop using**: Uninstalling the App and deleting all records stops data processing
- **Withdraw consent**: You can revoke microphone or speech recognition access anytime in your system settings; cloud transcription can still be used independently (to completely stop cloud uploads, avoid using the recording feature or contact us)

### 2.7 Data Retention

- Recordings and transcription data remain on your device and in your iCloud account until you delete them
- AI analysis and rewrite text is not stored on the server; it is released as soon as processing completes

### 2.8 Children's Privacy

The App is not intended for children under 13, and we do not knowingly collect personal information from children. If you believe we have unintentionally collected a child's information, please contact us for deletion.

### 2.9 Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be notified prominently within the App. The updated policy will be published on this page with the revised date.

### 2.10 Contact Us

If you have any questions or requests regarding this Privacy Policy, please contact us at:

- Email: 183835370@qq.com
- Effective date: August 13, 2026
