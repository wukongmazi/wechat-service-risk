# 微信支付服务商风险合规管理系统

https://mp.weixin.qq.com/s/ETtfLTgdQSPQerD7fL7KTA

![Image text](https://picx.zhimg.com/v2-bd36cfbe7ce73a10b8ffcba9e2d5257f_1440w.png?source=d16d100b)

#### 介绍
微信支付服务商风险合规包括处理子商户的消费者投诉和平台违规处置。无论是哪种，服务商都会及时收到通知。而是否帮助子商户自动处理则是有触发条件的。

大家好，我是小悟

![Image text](https://pic1.zhimg.com/80/v2-b2cc69be2ce282fe415abb355a9e159d_720w.png?source=d16d100b)

微信支付服务商风险合规包括处理子商户的消费者投诉和处理子商户的平台违规处置。

我们都知道，微信支付服务商可以拓展子商户，帮助商家在线下门店，小程序，公众号，移动应用app，网页等各个交易场景下使用微信支付进行收款满足商家不同场景下的支付诉求，让商家轻松接入微信支付。

玩过微信支付生态的，或许就有这种感受，如果收到消费者投诉单，不会通知到手机端，只会在微信支付商户后台-账户中心-消费者投诉那里显示。其实服务商可以帮助子商户自动及时处理这样的问题。

![Image text](https://pic1.zhimg.com/80/v2-23fa4dbfe5ad52d70d73ff82b92cff2f_720w.png?source=d16d100b)

再者，当子商户有新的违规、拦截（大于10次时）和申诉事件发生时，也不会通知到手机端，只会在微信支付商户后台-账户中心-违约记录那里显示。其实服务商也可以帮助子商户自动及时处理这样的问题。

![Image text](https://pic1.zhimg.com/80/v2-e4011c47e6ee923eb7ff6f80676c1426_720w.png?source=d16d100b)

![Image text](https://picx.zhimg.com/80/v2-5c378ffe7668d43658b8cf2b6feaeb72_720w.png?source=d16d100b)

![Image text](https://pica.zhimg.com/80/v2-a39f9ec46d7c933cb3c9797ac9653a62_720w.png?source=d16d100b)

搞了个系统来解决这两个问题，起码会比较及时处理。只要服务商的微信参数和通知参数配置正确，无论是消费者投诉还是平台违规处置，服务商都会及时收到通知。而是否帮助子商户自动处理则是有触发条件的。废话不多说，来看一下这个系统。

#### 消费者投诉

服务商可以帮助子商户快速获取其所属的消费者投诉问题并进行处理，提高子商户解决消费者投诉的处理能力及效率，为用户提供更优质的服务体验。

系统会做的操作是，给服务商和子商户及时发送消息通知、给用户回复消息、自动退款、关闭投诉单。

#### 平台违规处置

服务商可以帮助子商户获取到新的违规、拦截（大于10次时）和申诉事件通知，对服务商来说其实这是必要的，如果子商户违规了，作为服务商应该及时知晓并对子商户做出处理，相当于是一个风控子商户的功能。那对子商户来说，也可以及时收到拦截或申诉结果的通知。

违规记录通知：经过微信支付排查确认子商户有风险后，将会对子商户进行违规处置，处置发生时会发送至服务商。服务商可对子商户的违规处置进行排查或引导申诉。

拦截记录通知：若子商户的某一笔交易存在风险并且命中微信支付侧的风控策略，该订单就会被拦截，当同一子商户交易订单累计拦截数大于10笔时就会触发通知。单个子商户一天最多通知一次。

申诉单据通知：当子商户提交违规申诉后，会收到申诉变更通知。

系统会做的操作是，给服务商和子商户及时发送消息通知。

#### 商户信息

这里是对服务商所属子商户的管理，包括基本设置和通知设置。

![Image text](https://picx.zhimg.com/80/v2-408e0e4cc9347ef9232d5300460696a2_720w.png?source=d16d100b)

基本设置字段包括商户名称、商户号、商户回复用户内容、设置是否自动退款、设置状态。

![Image text](https://picx.zhimg.com/80/v2-def63c8bb39547eed774bd98c6dbb20d_720w.png?source=d16d100b)

当系统在收到子商户的用户投诉时会自动回复，回复的内容就是获取的【商户回复用户内容】字段的值，所以，这个字段填写的内容要友好、客气、礼貌一点，毕竟，客户可是上帝哦。

如果开启了自动退款，系统收到投诉单后，也会自动退款，然后将投诉单状态改为已处理完成。

如果将状态改为禁用，则子商户不会收到通知，也不会对投诉做任何的处理。

通知设置配置正确了，就可以及时通知到子商户，提供三种通知渠道选择，邮箱通知、公众号通知、短信通知。

![Image text](https://picx.zhimg.com/80/v2-de4b3167954598fa3574fefd5a358797_720w.png?source=d16d100b)

![Image text](https://pic1.zhimg.com/80/v2-58de32a7f2c351a9f6825d66b91e7a40_720w.png?source=d16d100b)

邮箱通知需要设置发送人邮箱(必须是网易云163邮箱)、发送人邮箱授权码、接收人邮箱。

公众号通知需要设置公众号appId、公众号secret、公众号模板消息id、接收人公众号openId。

短信通知需要设置腾讯云短信secretId、腾讯云短信secretKey、腾讯云短信模板id、腾讯云短信appId。

![Image text](https://pica.zhimg.com/80/v2-4a86ce83f67ab6fc9fd984011afb4a79_720w.png?source=d16d100b)

#### 微信管理

这里是对微信支付服务商参数的配置。

![Image text](https://picx.zhimg.com/80/v2-034ea02050f05ae6ad2282f4d9c0cd48_720w.png?source=d16d100b)

要准备商户名称、商户号、商户号绑定的appid、商户API证书序列号、微信支付平台证书序列号、商户API证书位置路径、微信支付平台证书位置路径、商户平台apiV3密钥，微信退款回调通知地址、回复用户内容(在系统中匹配不到子商户号时取该值内容回复)、设置是否自动退款(在系统中匹配不到子商户号时取该值内容判断)。

#### 通知管理

这里是对微信支付服务商通知参数的配置，所需通知渠道和参数和子商户的通知配置一样，就不再赘述。

![Image text](https://picx.zhimg.com/80/v2-0f32c12e4d3048b24f3f1bc004b9f7a2_720w.png?source=d16d100b)

#### 消费者投诉

这个设置很重要，能否及时处理投诉就看这个有没有设置成功。所填写的内容就是下面这个，但要记得把“域名”替换为当前系统的域名。

https://域名/prod-wxservicerisk-api/complaint/complaintbaseinfo/notify/complaintNotifyCallBack

![Image text](https://picx.zhimg.com/80/v2-582c895006d6f75afe7da09212c2e87c_720w.png?source=d16d100b)

#### 平台违规处置

这个设置也很重要，能否及时处理平台违规处置就看这个有没有设置成功。所填写的内容就是下面这个，但要记得把“域名”替换为当前系统的域名。

https://域名/prod-wxservicerisk-api/violation/violationbaseinfo/notify/violationNotifyCallBack

![Image text](https://picx.zhimg.com/80/v2-f5750bf89d1affd87bb817eb95c37b92_720w.png?source=d16d100b)

公众号后台回复【微信风险合规】获取账号密码。

![Image text](https://pic1.zhimg.com/80/v2-fc64ca6384d51bffb28eb6e100c1185c_720w.png)

山水有相逢，来日皆可期，谢谢阅读，我们再会

我手中的金箍棒，上能通天，下能探海