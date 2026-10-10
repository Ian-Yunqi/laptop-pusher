# 笔记本远程按键器

访问：https://ian-yunqi.github.io/laptop-pusher/

单文件静态控制网页，通过 Sites 网关连接 MQTT 服务。手机和电脑均可访问。

## 使用

1. ESP8266 接入能上网的 2.4GHz Wi-Fi，串口显示 `Cloud: ONLINE`。
2. 打开网页右上角设置，输入控制密钥，点击连接。
3. 等待“ESP 在线”后使用正转、停止、反转。没有原点开关时，圈数按运行时间估算，需实测校准。

控制密钥只保留在当前页面内存中，由网关验证。MQTT 账号密码保存在 Sites 后端的私密环境变量中，仓库不包含设备固件、Wi-Fi 密码或 MQTT 密码。

## 发布

GitHub Pages 从 main 分支根目录发布 `index.html`，更新此文件并提交即可自动部署。背景为 AI 生成的哥伦比娅同人插画，已内嵌在 HTML 中。
