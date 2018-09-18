Game Engine Frame
===============
一个跨平台的游戏服务器框架， 支持windows和linux下编译部署。
采用的是目前流行的多进架构，将不同的业务分布到不同的进程实例上，根据业务的不同， 
实例部署的个数也不同。

email : ylmbtm@163.com   QQ群 : 45139128 (加群后可以获取全部客户端代码和资源)

结构
===============
![结构](https://wx2.sinaimg.cn/mw690/79045675gy1fvbd68kd1uj20vv0rlmz8.jpg)

服务器说明
===============
### 1.登录服务器(LoginServer)
	说明: 接受玩家的登录连接， 处理登录请求消息

### 2.账号服务器(AccountServer)
	说明: 处理账号登录的验证，新账号的创建，账号的数据库保存

### 3.中心服务器(CenterServer)
	说明: 用于跨服活动， 跨服战需求

### 4.逻辑服务器(LogicServer)
	说明: 处理玩家角色的逻辑数据，处理玩家角色的一般逻辑功能。

### 5.战斗/副本/战场/服务器(GameServer)
	说明: 战场服务器， 副本，大世界，战斗的支持服务器， 处理玩家移动同步，技能，buff等作战功能。

### 6.DB服务器(DBServer)
	说明: 作为逻辑服和mysql数据库之间的代理服务器，负责定期将玩家的数据写入数据库。

### 7.网关服务器(ProxyServer)
	说明: 作为客户端和逻辑服，战场服之间的中转服务器，主要负责消息的转发。

### 8.日志服务器(LogServer)
	说明: 日志服务器 主要负责逻辑服运营日志的写入mysql数据库。

### 9.Http服务器(HttpServer)
	说明: http服务器， 主要负责php后台和游戏服务器之间的通信， 比如接受后台指令， 处理充值等等。

### 10.监视服务器(WatchServer)
	说明: 主要负责接受WEB后台的控制命令， 启动服务器， 关闭服务器，监视服务器状态,  更新服务器程序和配制。



体验客户端效果(加群可以获取全部客户端代码及资源)
===============
![login1](https://wx2.sinaimg.cn/mw690/79045675gy1fvdn1uoqa8j20pg0etabd.jpg)
![login2](https://wx2.sinaimg.cn/mw690/79045675gy1fvdn1uqpclj20wg0fxgn8.jpg)
![login3](https://wx4.sinaimg.cn/mw690/79045675gy1fvdn1uqq84j20wd0fydi0.jpg)
![login4](https://wx3.sinaimg.cn/mw690/79045675gy1fvdn1urjzaj20wd0gedia.jpg)
![login5](https://wx2.sinaimg.cn/mw690/79045675gy1fvdn1uq19vj20wh0fwdhn.jpg)