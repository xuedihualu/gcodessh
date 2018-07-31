# xuedihualu

sshgo

借助 GoldenPassport 实现 Mac 下 Google Authenticator 验证码自动输入


Usege


安装 GoldenPassport

GoldenPassport 是 Google Authenticator 的 Mac 版，具体功能可以通过：https://github.com/stanzhai/GoldenPassport 了解。它提供了 http 接口去获取 auth code，这为我们实现
更多充满想象力的功能提供了基础。安装包下载地址

添加验证码

可通过二维码或者 URL 的方式添加验证码

获取 verification code api

安装之后可在任务栏找到 GoldenPassport 的图标，打开 HTTP 服务，选择浏览器
访问 http://localhost:17304 ，在打开的页面中获取验证码对应的 api URL。

配置服务器列表

编辑 ssh.py 文件，配置 CONFIGS 和 AUTH_URL


相关命令
便捷使用
可将 ssh.py 放到 PATH(/usr/local/bin) 目录下，
赋予可执行权限：chmod +x /usr/local/bin/ssh.py 
这样在任何地方就能使用 ssh.py 命令快速登录服务器


Enjoy it
