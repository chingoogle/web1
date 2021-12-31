

部署完成后，每次启动应用时，运行的 web为最新版本

## 部署

### 步骤


> [![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/chingoogle/web1)

 4. 回到专案首页，点击上面的链接以部署 

### 变量

对部署时需设定的变量名称做如下说明。

| 变量 | 默认值 | 说明 |
| :--- | :--- | :--- |
| `ID` | `ad806487-2d26-4636-98b6-ab85cc8521f7` | VMess 用户主 ID，用于身份验证，为 UUID 格式 |
| `AID` | `64` | 为进一步防止被探测所设额外 ID，即 AlterID，范围为 0 至 65535 |
| `WSPATH` | `/` | WebSocket 所使用的 HTTP 协议路径 |

## 接入 CloudFlare

以下两种方式均可以将应用接入 CloudFlare，从而在一定程度上提升速度。

 1. 为应用绑定域名，并将该域名接入 CloudFlare
 2. 通过 CloudFlare Workers 

## 注意

不要封禁web
