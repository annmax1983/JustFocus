# JustFocus
[English](../README.md) | 中文 | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

一款轻量级浏览器扩展，屏蔽干扰网站，帮助你保持专注。极简、快速、隐私优先。

> Chrome / Edge / Firefox · Manifest V3 · 最小权限 · 本地优先 · 无追踪

---

## 功能特性

| 功能 | 说明 |
|------|------|
| 🚫 **自定义屏蔽列表** | 添加任意域名，自动覆盖其所有子域名 |
| 🔄 **全局开关** | 一键切换所有屏蔽的开/关状态 |
| ⏱️ **5 分钟临时解锁** | 临时访问被屏蔽的网站，5 分钟后自动重新屏蔽 |
| 💾 **同步存储** | 屏蔽列表在浏览器账号间同步（Chrome / Edge / Firefox） |
| 🛡️ **MV3 原生** | 使用 declarativeNetRequest，无旧版 API |
| 🌐 **自动语言** | 检测浏览器语言，默认英文 |
| 📋 **完整列表页** | 管理所有屏蔽站点、修改时长、导出与导入 |
| 🔑 **密码保护** | 可选的本地密码：解除屏蔽、移除站点、关闭总开关都需要输入密码。忘记密码无法找回 |
| ⭐ **Pro 版** | 外科式屏蔽——只隐藏 Shorts、Reels 与推荐流，站点其余功能照常使用（一次性 VKT Pro 版许可证） |

---

## 免费 vs Pro 版

| 版本 | 屏蔽站点 | 导出 / 导入 | 外科式屏蔽 |
|------|---------|------------|-----------|
| **免费版** | 不限数量 | 支持 | 仅 YouTube Shorts |
| **⭐ Pro 版** | 不限数量 | 支持 | 全部 12 个支持站点 |

屏蔽网站本身**完全免费、站点数量不限**。**Pro 版解锁「外科式屏蔽」**——只隐藏最上瘾的那部分（Shorts、Reels、推荐流），站点其余功能照常使用，覆盖 YouTube、Instagram、TikTok、Facebook、Reddit、X、Pinterest、Threads、LinkedIn、Snapchat、VK、小红书。

> YouTube Shorts 的屏蔽对所有用户免费，其余站点需要Pro 版许可证。

- 🛒 获取许可证：`https://annmax1983.com/checkout?plugin=justfocus`
- ⚙ 激活：打开 JustFocus 弹窗 → 点击 **⚙ / 🔒** 按钮 → 输入许可证密钥。

> 许可证激活是**可选的**。免费版无需任何账号、注册或许可证即可完整使用。

---

## 支持的浏览器

| 浏览器 | 状态 |
|--------|------|
| Google Chrome | ✅ 完全支持 |
| Microsoft Edge | ✅ 完全支持 |
| Mozilla Firefox | ✅ 完全支持 |
| 其他 Chromium 内核浏览器 | ✅ 应该可用 |

> **Firefox 说明：** Firefox for Android 版暂未启用（清单未声明 `gecko_android`），AMO 上目前只提供桌面版。其余功能与 Chrome / Edge 一致。

---

## 安装

| 商店 | 链接 |
|---|---|
| Chrome 应用商店 | [在 Chrome 中安装](https://chromewebstore.google.com/detail/iocnhglbdkdonajhkipknhgdnbombcic) |
| Microsoft Edge 加载项 | [在 Edge 中安装](https://microsoftedge.microsoft.com/addons/detail/eigeengnoahojmfcnkkjnipbdnpngaod) |
| Firefox 附加组件（AMO） | [安装 Firefox 版](https://addons.mozilla.org/firefox/addon/justfocus/) |

> 请只通过上方官方商店安装，避免使用第三方下载站。

---

## 使用方法

### 屏蔽网站

1. 点击 JustFocus 图标
2. 输入域名（如 `youtube.com`）
3. 按回车或点击 **+**
4. 完成 — 访问该网站时将跳转到专注提醒页面

### 临时解锁

1. 跳转到被屏蔽页面时，点击 **"解锁 5 分钟"**
2. 立即跳转到该网站
3. 5 分钟后自动恢复屏蔽

### 暂停所有屏蔽

- 将弹窗顶部的开关切换到 OFF
- 所有网站立即解除屏蔽
- 切换回 ON 重新启用

### 密码保护（可选）

管不住自己手滑点"解锁"？设置一个密码：

1. 打开弹窗 → 点击 **⚙ / 🔒** → *密码保护* 区块，或在列表页点击 🔒 按钮
2. 设置密码（至少 4 位）——只保存加盐哈希，不是密码本身。和其他设置一样存在 Chrome 存储里，开启浏览器同步时会随同步走，但不会发到 JustFocus 服务器
3. 此后以下操作都需要输入密码：
   - 关闭总开关
   - 屏蔽页上的"解锁 5 分钟"
   - 移除站点或清空列表
   - 修改屏蔽时长
4. 随时可以修改或移除密码（需要当前密码）

> ⚠️ **忘记密码将无法找回。** 没有重置链接、没有找回渠道、没有后门——这是刻意设计。请选择一个你记得住的密码。

---

## 隐私

- **declarativeNetRequest** — 使用声明式规则屏蔽网站，不读取页面内容
- **storage** — 本地保存屏蔽列表，不上传数据
- **密码（可选）** — 设置密码后，只保存加盐哈希，不保存明文。和其他设置一样存放在 Chrome 存储中，开启浏览器同步时可能在你设备之间同步；不会发到 JustFocus 服务器。忘记密码无法找回。
- **alarms** — 管理临时解锁定时器，无后台追踪
- **许可证（可选）** — 仅当您激活付费许可证时，会向 `api.annmax1983.com` 发送许可证密钥、随机安装标识和浏览器元数据，用于激活/校验许可证。绝不包含您的屏蔽列表、浏览历史或个人数据。
- 使用 `<all_urls>` 主机权限仅用于 declarativeNetRequest 屏蔽规则，授权服务器仅用于付费激活。无追踪，无分析。免费功能不联络任何 JustFocus 服务器；屏蔽列表与设置保存在浏览器存储中，只有你自行开启浏览器账号同步时才会由浏览器复制到其他设备。

---

## 版权声明

本扩展仅在本地屏蔽用户指定的网站，帮助用户在工作或学习时保持专注。扩展不修改、复制或重新分发任何网站内容。所有网站内容版权归原始发布者所有。

---

## 源码说明

> ⚠️ **本仓库仅用于项目展示，不发布完整源码。** 这里只有扩展的使用说明、更新日志与支持信息。

> 📥 **请前往官方浏览器商店下载安装：** Chrome Web Store · Microsoft Edge Add-ons · Firefox 附加组件（AMO）。本仓库不提供离线安装包，也不向终端用户分发源码包。

---

## 许可证

Copyright © 2026 JustFocus. 保留所有权利。

本软件为闭源专有软件。未经作者书面授权，严禁反编译、逆向工程、破解、修改、重新打包、再分发或转售本软件（含全部或部分）。

---

## 链接

- **官方网站:** https://annmax1983.com/
- **本插件:** https://annmax1983.com/extensions/justfocus
- **隐私政策:** https://annmax1983.com/privacy
- **联系:** support@annmax1983.com
- **☕ 支持这个项目（Ko-fi）:** https://ko-fi.com/annmax?ref=justfocus
