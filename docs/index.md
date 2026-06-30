---
title: "开发者文档"
nav_order: 2
permalink: "/docs/"
---

# Topo 链 DApp 开发者最佳实践文档
{: .no_toc }

为便于 GitHub Pages 发布和阅读，本文档已按工程主题聚合为 6 个章节。每个章节保留原始内容的标题、表格、检查清单和 Mermaid 图，但减少左侧导航层级。
{: .fs-6 .fw-300 }

## 阅读路径

- [1. 总览、原则与工程架构]({% link docs/01-overview-architecture.md %})：先建立文档定位、核心工程原则和推荐系统架构，帮助团队统一链上事实、链下服务和 POC 边界。
- [2. 链上合约、状态机与事件契约]({% link docs/02-contract-state-events.md %})：聚焦 Move 合约模块拆分、状态机、事件契约和 view 设计，这是 DApp 可信事实的核心。
- [3. 交易入口、事件同步与读模型]({% link docs/03-transaction-sync-read-model.md %})：把 signed transaction 入口校验、API 到 ABI 清单、event_bus 消费和读模型投影放在同一章，形成完整链下处理闭环。
- [4. POC 接入与 Web3 商城案例]({% link docs/04-poc-integration-marketplace-case.md %})：先说明 DApp 侧 POC 贡献链路，再用 Web3 商城案例落到支付、履约、结算和贡献发放。
- [5. 安全、测试与可观测性]({% link docs/05-security-testing-observability.md %})：把钱包登录、资产金额、权限暂停、测试矩阵、监控指标和对账视图合并为质量保障章节。
- [6. 上线清单、反模式与开发顺序]({% link docs/06-launch-antipatterns-roadmap.md %})：面向发布和交付阶段，汇总上线检查、常见反模式、开发顺序和最终边界总结。

## 聚合关系

| 聚合章节 | 原始章节 | 聚合理由 |
|---|---|---|
| [1. 总览、原则与工程架构]({% link docs/01-overview-architecture.md %}) | 0. 文档定位<br>1. 核心工程原则<br>2. 推荐工程架构 | 先建立文档定位、核心工程原则和推荐系统架构，帮助团队统一链上事实、链下服务和 POC 边界。 |
| [2. 链上合约、状态机与事件契约]({% link docs/02-contract-state-events.md %}) | 3. 链上合约设计 | 聚焦 Move 合约模块拆分、状态机、事件契约和 view 设计，这是 DApp 可信事实的核心。 |
| [3. 交易入口、事件同步与读模型]({% link docs/03-transaction-sync-read-model.md %}) | 4. Signed Transaction 入口设计<br>5. 事件同步和读模型 | 把 signed transaction 入口校验、API 到 ABI 清单、event_bus 消费和读模型投影放在同一章，形成完整链下处理闭环。 |
| [4. POC 接入与 Web3 商城案例]({% link docs/04-poc-integration-marketplace-case.md %}) | 6. POC 接入最佳实践<br>7. Web3 商城参考案例 | 先说明 DApp 侧 POC 贡献链路，再用 Web3 商城案例落到支付、履约、结算和贡献发放。 |
| [5. 安全、测试与可观测性]({% link docs/05-security-testing-observability.md %}) | 8. 安全最佳实践<br>9. 测试矩阵<br>10. 可观测性和对账 | 把钱包登录、资产金额、权限暂停、测试矩阵、监控指标和对账视图合并为质量保障章节。 |
| [6. 上线清单、反模式与开发顺序]({% link docs/06-launch-antipatterns-roadmap.md %}) | 11. 上线检查清单<br>12. 常见反模式<br>13. 开发顺序建议<br>14. 总结 | 面向发布和交付阶段，汇总上线检查、常见反模式、开发顺序和最终边界总结。 |
