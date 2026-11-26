# Proxy_Suite_Modules

Proxy Suite 自维护 App 去广告远程模块仓库，托管无第三方作者覆盖或上游模块存在缺陷的独立单 App 增强模块。坚持“一 App 一独立模块”，不做大合集；三端模块标题统一采用与 App 原图标配色对齐的 Emoji 标识（可选附带自托管 PNG 图标），方便客户端直观辨识、单独开关与独立更新。

## 模块列表

| App | 说明 | MitM 域名 | Stash 一键安装 | Surge | Stash | Shadowrocket |
| --- | --- | --- | --- | --- | --- | --- |
| <img src="icons/Dingdong.png" width="24" alt="叮咚买菜"> 叮咚买菜 | 拦截叮咚买菜开屏、开屏预加载与首页弹窗广告；保留绿卡会员与正常购物接口。 | `maicai.api.ddxq.mobi` | [一键安装](https://link.stash.ws/install-override/raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/Dingdong.stoverride) | [Dingdong.sgmodule](surge/Dingdong.sgmodule) | [Dingdong.stoverride](stash/Dingdong.stoverride) | [Dingdong.srmodule](shadowrocket/Dingdong.srmodule) |
| <img src="icons/McDonalds.png" width="24" alt="麦当劳"> 麦当劳 | 拦截麦当劳开屏排期（返回空日程 data.list=[]）与首页活动弹窗广告；保留点餐、会员与正常业务接口。 | `api.mcd.cn` | [一键安装](https://link.stash.ws/install-override/raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/McDonalds.stoverride) | [McDonalds.sgmodule](surge/McDonalds.sgmodule) | [McDonalds.stoverride](stash/McDonalds.stoverride) | [McDonalds.srmodule](shadowrocket/McDonalds.srmodule) |

## 远程订阅与一键安装

### 🥬 叮咚买菜

- Stash 一键安装（GitHub 页面可直接点击）：[点击直接拉起 Stash 安装](https://link.stash.ws/install-override/raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/Dingdong.stoverride)
- Stash 原始链接：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/Dingdong.stoverride`
- Surge 原始链接：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/surge/Dingdong.sgmodule`
- Surge URL Scheme 唤起（复制到 Safari 地址栏或 iOS 备忘录点击）：`surge:///install-module?url=https%3A%2F%2Fraw.githubusercontent.com%2FAnTong-Git%2FProxy_Suite_Modules%2Fmain%2Fsurge%2FDingdong.sgmodule`
- Shadowrocket 原始链接：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/shadowrocket/Dingdong.srmodule`
- 图标文件：[Dingdong.png](icons/Dingdong.png)（`https://fastly.jsdelivr.net/gh/AnTong-Git/Proxy_Suite_Modules@main/icons/Dingdong.png`）

### 🍟 麦当劳

- Stash 一键安装（GitHub 页面可直接点击）：[点击直接拉起 Stash 安装](https://link.stash.ws/install-override/raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/McDonalds.stoverride)
- Stash 原始链接：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/McDonalds.stoverride`
- Surge 原始链接：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/surge/McDonalds.sgmodule`
- Surge URL Scheme 唤起（复制到 Safari 地址栏或 iOS 备忘录点击）：`surge:///install-module?url=https%3A%2F%2Fraw.githubusercontent.com%2FAnTong-Git%2FProxy_Suite_Modules%2Fmain%2Fsurge%2FMcDonalds.sgmodule`
- Shadowrocket 原始链接：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/shadowrocket/McDonalds.srmodule`
- 图标文件：[McDonalds.png](icons/McDonalds.png)（`https://fastly.jsdelivr.net/gh/AnTong-Git/Proxy_Suite_Modules@main/icons/McDonalds.png`）

## 使用说明

- Stash 一键安装通过 Stash 官方 HTTPS 中转链接 `link.stash.ws` 302 跳转至 `stash://install-override?url=...` 拉起客户端安装单个覆写，保存后仍从 GitHub 原始地址自动更新。
- Surge 因 GitHub 网页版过滤自定义协议，可在手机上复制对应的 `surge:///install-module?url=...` 到 Safari 地址栏或 iOS 备忘录轻点拉起，或直接复制 `.sgmodule` 原始链接在 Surge「模块」中粘贴添加。
- Shadowrocket 请在「配置 → 模块 → +」中粘贴对应 `.srmodule` 原始链接；请勿导入整份仓库说明文件。
- 所有模块按「一 App 一模块」独立维护，按需单独安装与启用；启用后需同时信任对应客户端的 MITM 根证书，仅对模块声明的精确业务域名生效。
- 本仓库仅作远程分发镜像，源定义与校验由主工程统一生成与维护。
