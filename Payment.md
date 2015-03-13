支付方案选择。


&lt;BR&gt;




1. 市场主要解决方案

京东采用了腾讯的财付通、快钱、CMPAY、汇付天下（chinapnr.com），银联支付（尚未开通）。


易迅网采用了腾讯财付通、快钱、支付宝即时到账、环讯支付IPS（上海本地）




其他医疗网站


&lt;BR&gt;





&lt;BR&gt;



2.其他医疗健康网站采用的支付方式
1． 好大夫采用纯手工方式。
> ![http://ttdong.googlecode.com/files/haodf.jpg](http://ttdong.googlecode.com/files/haodf.jpg)


3.选择标准

选择的标准主要有：手续费比例、一次性费用、结算速度、

支付宝：

快钱：


> 手续费	网址	备注
支付宝	1.2%	http://act.life.alipay.com/shopping/before/help/index.html

快钱	签约后才知道	http://club.99bill.com/viewthread.php?tid=40035
财付通	签约后才知道	http://mch.tenpay.com/



快钱联系方式：

地址：上海市浦东新区世纪大道1600号（浦电路路口）陆家嘴商务广场29楼 邮编：200122
ADD: 29th floor, LJZ PLAZA, 1600 Century avenue, Pudong, Shanghai, China

TEL: 86-21-58779699　 86-21-61871299
FAX: 86-21-58779099



&lt;BR&gt;


4.架构
因为支付的方法都差不多。
构造提交到支付平台的各种参数 –》跳转到支付平台支付平台用户支付支付成功后支付平台回调我方API。

所以针对每种支付平台
需要实现部分：
1）	构造URL参数或者Post数据（一般包括订单号、金额、userid、usertoken、加密算法等）
2）	编写一个API，供支付平台回调。API中要校验回调数据合法性、然后修改订单状态，纪录历史纪录。


所以对架构上的要求：
1）	支付方法的添加、修改是一个可扩展的架构。比如要增加一个新的支付方法，就只需要添加一些新的配置文件，然后contribute一些代码即可。不需要修改原有支付方法代码。
2）	能进行容错处理。

下面是支付宝API的example code:

http://club.alipay.com/read.php?tid=9976972

选择“支付宝即时到账收款接口 ”



推荐支付宝：因为初期业务量不大，相对来说支付宝集成比较容易。