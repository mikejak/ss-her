Fork 于 shadowsocks-heroku 项目

shadowsocks-heroku
Heroku 是一个支持多种编程语言的云平台即服务，shadowsocks-heroku 则是可部署在 Heroku 平台的 ss 服务。 和 shadowsocks 不同的是 shadowsocks-heroku 使用的 WebSocket 代替原本的 sockets。

如果遇到问题
请先检查是否遵循步骤（再次阅读一遍教程）
请先自行通过搜索引擎寻找答案
如果还没有解决，欢迎创建 issue 提问（贴日志和配置的时候注意隐藏app地址和密码等敏感信息）
准备
1. 注册 Heroku 帐号
Heroku 提供免费账号，部分介绍如下：

512 MB RAM per dyno
Free apps sleep automatically after 30 mins of inactivity to conserve your dyno hours
Free apps wake automatically when a web request is received
https://devcenter.heroku.com/articles/limits
用作 VPS 是够了，注册地址：https://signup.heroku.com/

部署
点击  , 一键部署到heroku

设置 加密算法和app 密码 deploy


支持的加密算法类型如下https://github.com/mrluanma/shadowsocks-heroku#supported-ciphers

启动本地 Client
下载release https://github.com/onplus/shadowsocks-heroku/releases （备份）

修改config.json参数（主要是server，password和method），运行ss-h

启动成功，命令行显示：server listening at { address: '127.0.0.1', family: 'IPv4', port: 1080 }

配置代理
下载：Chrome 浏览器 SwitchyOmega 插件

安装：打开浏览器的扩展程序页面 chrome://extensions，把 SwitchyOmega.crx 文件拖放到浏览器扩展程序页面安装

配置：SwitchyOmega

代理协议：SOCKS5
代理服务器：127.0.0.1
代理端口：1080
   ```

可选：
使用无污染DNS https://www.zhihu.com/question/32229915
cow/meow  https://github.com/cyfdecyf/cow#cow-climb-over-the-wall-proxy
送人玫瑰手留余香rose（原作者）
