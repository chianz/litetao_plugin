# 油猴插件：在PC查询特价淘宝的订单
淘宝在2020年10月中旬上线了一个的功能：特价淘宝下的订单不能在淘宝里查询！
这傻X的功能真是让人恼火，几百个订单里要在这小屏的手机上滚下滚地找...太不方便了。
于是抓了一下数据接口，把数据弄到PC上显示。

简单的jQuery实现，订单列表基本仿原生样式


**使用方法:**

[已装油猴插件的话，点击安装](https://raw.githubusercontent.com/machinewu/litetao_plugin/master/litetao_plugin.user.js)

![使用效果图片](https://user-images.githubusercontent.com/4166753/99198190-e8a97580-27d1-11eb-99a3-c4d951719dc7.png)


**存在问题:**
- 由于订单列表查询接口没有返回订单时间和确认收货的剩余时间，所以列表默认是不显示这两项的
- 曾经尝试过用订单详情接口查这两项数据，但是由于查询过频繁，会被系统block请求。所以最终决定不查这两项了。
- 将鼠标移动到“查看物流”，就会填充这两项。确认收货的剩余时间是自己算的，会有偏差，真实的时间请点进去“查看物流”看。

