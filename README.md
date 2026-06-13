# HayGorNoClash

这是一个为 Clash 设计的定制配置文件。

## 项目特点

- **规则源切换**：已从 `Loyalsoldier/clash-rules` 迁移至 `dler-io/Rules`，提供更精准的规则分流。
- **自动化规则提供者**：利用 Clash 的 `rule-providers` 功能，支持规则集的自动更新（24小时周期）。
- **优化分流策略**：
    - **广告拦截**：使用 `AdBlock` 规则集。
    - **苹果服务**：独立分流以优化 App Store 和 iCloud 体验。
    - **AI 服务**：专门针对 OpenAI (AI Suite) 的规则配置。
    - **国内直连**：精准识别国内域名及 IP。
    - **流媒体优化**：针对 Netflix、Disney+ 等平台。

## 核心配置

主配置文件：`HayGorNoClash.yaml`

### 规则提供者 (Rule Providers)

目前配置使用了 `dler-io/Rules` 仓库中的以下模块：
- `Proxy`: 全球代理规则
- `Domestic`: 国内直连域名
- `Domestic IPs`: 国内 IP 段
- `AdBlock`: 广告过滤
- `Apple`: 苹果全家桶
- `AI Suite`: OpenAI / Claude 等 AI 工具
- `Telegram`: 电报即时通讯

## 如何使用

1. 确保你安装了支持 Rule Provider 的 Clash 客户端（如 Clash Premium, Clash Verge, Clash Meta 等）。
2. 将 `HayGorNoClash.yaml` 导入你的客户端。
3. 规则集会自动从 jsDelivr CDN 下载并定期更新。

## 维护记录

- **2026-06-13**: 初始化 Git 仓库。
- **2026-06-13**: 将所有规则源从 Loyalsoldier 迁移至 dler-io，并适配 `classical` 行为模式。
