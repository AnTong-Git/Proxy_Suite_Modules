# Proxy_Suite_Modules

Proxy Suite 自维护 App 去广告远程模块仓库，托管无第三方作者覆盖的 App 增强模块。

## 模块列表

| App | 说明 | MitM 域名 | Surge | Stash | Shadowrocket |
| --- | --- | --- | --- | --- | --- |
| 叮咚买菜 | 拦截叮咚买菜开屏、开屏预加载与首页弹窗广告；保留绿卡会员与正常购物接口。 | `maicai.api.ddxq.mobi` | [Dingdong.sgmodule](surge/Dingdong.sgmodule) | [Dingdong.stoverride](stash/Dingdong.stoverride) | [Dingdong.srmodule](shadowrocket/Dingdong.srmodule) |

## 远程订阅链接

### 叮咚买菜

- Surge：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/surge/Dingdong.sgmodule`
- Stash：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/stash/Dingdong.stoverride`
- Shadowrocket：`https://raw.githubusercontent.com/AnTong-Git/Proxy_Suite_Modules/main/shadowrocket/Dingdong.srmodule`

## 使用说明

- 请勿克隆或导入整份仓库说明文件，按所用客户端在「模块 / 覆写」中粘贴对应原始链接即可。
- 启用模块后需同时信任对应客户端的 MITM 根证书，仅对模块声明的精确业务域名生效。
- 本仓库仅作远程分发镜像，源定义与校验由主工程统一生成与维护。
