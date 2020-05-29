1、服务器购买

使用vultr服务器进行搭建。[vultr官网](https://my.vultr.com/)，

vultr需要先在账户中充值金额，然后选择一款服务器，每个月从账户中扣除使用费用

目前新用户充值优惠满$10赠送$100，有效期30天，意味着30天内可以从赠送金额中扣除，超过30天则从本账户中扣除。

选择最便宜的即可，本教程中选择cloud compute，Los Angeles，Debian9，$5.00/mon的服务器，平均$0.007/hr。完成后点击Deploy now部署服务器。

2、域名购买和解析

通过国际老牌的域名服务商[namesilo](https://www.namesilo.com/)购买，有很多优惠的域名可供选择，本教程所使用的.xyz域名价格$0.9一年。

进入下·

3、v2ray搭建

github上有很多一件搭建的脚本，使用起来非常方便，而且是开源脚本。例如<https://github.com/233boy/v2ray/wiki>。如果不想具体了解可以参考下面简单流程：

使用Xshell连接服务器

下载并运行v2ray脚本

```
bash <(curl -s -L https://git.io/v2ray.sh)
```

根据脚本，选择4，webSocket+TLS，接下来根据提示选择

通过```v2ray status```查看运行状态，正确状态显示如下

> V2Ray 状态: 正在运行  /  Caddy 状态: 正在运行

4、v2ray客户端搭建

使用v2ray客户端v2rayN

下载链接：[ https://github.com/2dust/v2rayN/releases/latest](https://github.com/2dust/v2rayN/releases/latest)

如果使用上面连接下载过慢，可自行选择其他资源

1）在xshell执行```v2ray url```，获取连接

2）v2rayN中选择田间VMess服务器---从剪贴板导入URL

3）参数配置 本地监听端口2333

4）启动系统代理。选择PAC模式

