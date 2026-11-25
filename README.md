# 蜻蜓 Dragonfly · iOS Rime 输入法

iOS 第三方中文输入法。librime 引擎直接跑在键盘扩展进程里，没有服务端、没有进程间通信，离线可用。

本仓库用于**问题反馈与发布说明**，不包含源码。

## 特性

- **引擎在设备上**：librime + librime-lua + librime-octagram 静态链接进 App 与键盘扩展，断网照常打字
- **方案包按需下载**：雾凇拼音（全拼 / 自然码双拼）、万象拼音（多输入类型，含辅助码）
- **三套主题**：素翼、夜航、晨光，主 App 即时切换
- **中文打字手感**：26 键布局、连续滚动候选栏、滑选、长按符号、中英与输入方案独立切换
- **系统要求**：iOS 16.0 及以上；iPhone 与 iPad（分屏与浮动键盘留待 V1.1）

## 隐私

- 输入内容不出设备。不收集、不上传按键、候选与组码。
- 「允许完全访问」可选，**不开也能完整打字**。开启后目前只用于：按键触感反馈、跨会话保存学到的词。
- 联网只发生在两件事上：下载方案包与语法模型、检查更新。

## 反馈问题

- 提交 Issue：<https://github.com/CaicoLeung/dragonfly-app/issues>
- 提交前先看 App 内「通用 › 帮助与自检」与「宿主 App 兼容性」，多数常见情况在那里。
- 报问题时请附：机型与 iOS 版本、蜻蜓版本、使用中的方案包与输入方案、复现步骤。
- App 内「通用 › 反馈问题 › 导出诊断包」可导出：librime 版本、方案包与版本、输入方案 id、安装日志。诊断包**不含任何输入内容**。

## 许可与致谢

| 组件 | 许可 |
|---|---|
| librime / librime-lua / librime-octagram | BSD-3-Clause |
| OpenCC | Apache-2.0 |
| KeyboardKit 7.8.0（Hamster 快照） | MIT |
| 雾凇拼音 rime-ice | GPL-3.0 |
| 万象拼音 rime-wanxiang | CC BY 4.0 |
| 语法模型 rime-wanxiang-data | CC BY 4.0 |

各随安装内容落地的许可全文可在 App 内「通用 › 许可全文」查看。

## 状态

开发中，尚未上架 App Store。
