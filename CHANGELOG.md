# 更新日志

iNTM 的所有重要变更都将记录在此文件中。

格式基于 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.0.0/)，
项目遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

---

## [1.4.0] - 2026-01-29

### 新增
- 🗺️ **程序级连接详情视图**：支持查看每个应用的所有网络连接详情，包括 IP 地址、端口、协议、域名等完整信息
- 🌍 **地图可视化模式**：在世界地图上直观展示网络连接的地理位置分布，让全球网络活动尽在掌握
- 🎯 **支持隐藏 Dock 栏图标**：可选择仅在菜单栏显示，节省 Dock 栏空间，提供更简洁的桌面体验

### 优化
- ⚡ **锁机制性能优化**：将 NSLock 替换为 OSAllocatedUnfairLock，核心锁性能提升 3-4倍（从 40ns 降至 10ns）
- 🧹 **内存泄漏修复**：修复多处内存泄漏问题，显著降低长时间运行时的内存占用
- 🏗️ **架构优化改进**：代码重构，删除 376 行冗余代码（DNS 缓存模块），提升整体稳定性和可维护性
- 🗑️ **代码清理**：移除未使用的 DNS 统计功能、DNSCacheManager、DNSPacketParser 等死代码

### 修复
- 🐛 修复网络连接类型获取异常问题
- 🔧 修复 Swift 6 并发警告（NSXPCConnection Sendable conformance）
- 🔒 修复 FilterProviderXPCClient 原子性问题，确保线程安全

---

## [1.3.0] - 待补充

### 新增
- 待补充

### 优化
- 待补充

### 修复
- 待补充

---

## [1.2.0] - 待补充

### 新增
- 待补充

### 优化
- 待补充

### 修复
- 待补充

---

## [1.1.0] - 待补充

### 新增
- 待补充

### 优化
- 待补充

### 修复
- 待补充

---

## [1.0.0] - 待补充

### 新增
- 首次发布
- 系统级网络流量监控
- 实时速度显示
- 应用级别统计
- 待补充更多功能

---

## 版本说明

### 版本号规则

遵循 [语义化版本 2.0.0](https://semver.org/lang/zh-CN/)：

- **主版本号（Major）**：不兼容的 API 变更
- **次版本号（Minor）**：向下兼容的功能性新增
- **修订号（Patch）**：向下兼容的问题修正

### 变更类型

- `新增` - 新增功能
- `优化` - 性能或体验优化
- `修复` - Bug 修复
- `变更` - 功能调整或重构
- `移除` - 移除的功能
- `弃用` - 即将移除的功能

---

<!--
说明：
1. 请从官网 https://intm.jsiqi.vip/ 的版本更新日志中获取实际内容
2. 或根据 git commit 历史补充每个版本的具体变更
3. 建议包含：新功能、性能优化、Bug 修复、已知问题等
-->

[1.4.0]: https://github.com/yourusername/iNTM/releases/tag/v1.4.0
[1.3.0]: https://github.com/yourusername/iNTM/releases/tag/v1.3.0
[1.2.0]: https://github.com/yourusername/iNTM/releases/tag/v1.2.0
[1.1.0]: https://github.com/yourusername/iNTM/releases/tag/v1.1.0
[1.0.0]: https://github.com/yourusername/iNTM/releases/tag/v1.0.0
