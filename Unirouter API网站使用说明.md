本文档为Unirouter API网站使用说明

base url：https://unirouter.link

新用户可以根据下面介绍的速通指南快速上手👇

# 1. 快速接入

可按以下步骤快速接入Unirouter API：

注册/登录 ->  创建密钥 -> 调用API接口

1.1 注册/登录

登录网页进行注册或登录：https://unirouter.link/login

1.2 创建密钥

 控制台 -> API 密钥 -> 创建API密钥 

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701445/image-preview)

给密钥取一个名字，分组可以使用默认的auto分组，这样一个密钥可以同时支持所有模型的使用。

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701446/image-preview)

之后点击 保存更改 即可。（模型限制列表不要填写，保持空白即可）

**关于令牌分组**
- 不同分组里有不同模型，比如codex分组里只有gpt的codex模型，claude分组里面是claude的模型。
- 不同分组对应不同折扣，比如claude特价分组的模型费用折扣是1.9折，claudecode分组折扣是5.5折
- 如果不知道如何选择，建议直接选择auto分组，该令牌可以自动匹配到最优折扣的可用分组和模型。
- 如果对模型有特定要求，比如希望在claude code里使用，并且能够有较高的缓存命中，则可以选择claudecode分组。

如何查看不同分组里有什么模型？

选择模型广场 ( https://unirouter.link/pricing )，在可用令牌分组里选择你想看的分组，右边就会显示出当前所选分组包含的可用模型，如下图：

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701448/image-preview)

关于令牌额度：

令牌额度并非账号金额，而是对这个令牌可使用金额做的限制，如果令牌限额达到，即便账号还有余额，该令牌也无法使用。

如果不需要限制，建议直接选择设为无限额度

1.3 使用令牌

令牌创建完成后，点击令牌右边的复制按钮即可复制令牌，

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701450/image-preview)

使用以下信息即可完成大模型API相关的配置

Base URL: https://unirouter.link

API key：就是您刚才复制的令牌


# 2. 其他功能

2.1 游乐场

进入 控制台 -> 游乐场，可以选择各种大模型进行对话，提供了基本的对话功能。右下角可以切换不同模型。

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701451/image-preview)

2.2 数据看板

进入 控制台 -> 数据看板，可以查看账号状态，账号余额，数据统计，服务可用性等等

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701452/image-preview)

2.3 使用日志

进入 控制台 -> 使用日志，可以查看详细的大模型调用记录，可以按日期筛选

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701453/image-preview)

2.4 钱包管理

进入 控制台 -> 钱包，可以对您的账号钱包进行管理

在这里您可以选择两种充值方式

2.4.1 包月套餐

目前有三种包月套餐提供，套餐可叠加购买，互不干扰。

不同包月套餐对应的使用额度不同，并不是无限量使用，也不会提供重置，但是享有比普通的钱包充值更高的折扣。

**注意：包月套餐有效期一个月，到期后剩余额度即作废，请按需购买**

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701454/image-preview)

2.4.2 额度充值

在这里您可以按您的实际需要选择充值金额，不同充值金额也可以享受不同的充值折扣优惠

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701455/image-preview)

可以选择 Waffo 或者 Stripe 进行付款，此为第三方付款平台，会进行页面跳转，是正常情况。

平台上可以选择微信或者支付宝进行支付。

2.5 个人设置

进入 控制台 -> 个人设置，可以进行账号设置，比如绑定邮箱，余额提醒，语言选择等

![image.png](https://api.apifox.com/api/v1/projects/7041221/resources/701456/image-preview)


# 3. 常见问题

- 如何选择分组

建议使用默认的auto分组，可以一个key使用所有模型

- 是否有折扣？

请查看2.4节 钱包管理


- 如何查看模型价格

在模型广场里（https://unirouter.link/pricing）， 点开任何模型就可以看到不同分组对应的价格，所有价格已经在官方价格基础上按照折扣倍率进行打折，auto分组的令牌会自动选择最优分组。

- base url地址是？

base url地址是：https://unirouter.link

注意有些软件需要添加/v1：https://unirouter.link/v1

具体建议询问 AI 帮您确认
