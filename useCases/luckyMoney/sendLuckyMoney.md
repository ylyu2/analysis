### 描述

用户在频道中发送红包，让其他人来抢

### 角色

发红包的用户

### 触发

当用户想要发红包时

### 数据输入（来源）

1. 红包金额（发红包的用户）

2. 红包个数（发红包的用户）

### 数据输出（去向）

1. 红包是否创建成功（频道中的所有用户）


### 路径

1. “发红包的用户”输入指令```xxx 发红包 100 10```，其中100表示金额，10表示红包个数。（数据输入： #1、#2）
2. “Bot”检查“发红包的用户”的余额是否足够
3. “Bot”在“发红包的用户”扣除其金额。
4. “Bot”在后台创建一个红包。
5. “Bot”在该频道发送```user_name的红发已发出，大家快来抢```，user_name指代用户名。（数据输出：#1）
6. “Bot”在#5步骤中的消息添加一个“💰”Reaction。


### 扩展路径

2. 
	1. 如果余额不足
		1.  “Bot”回复到```user_name，你的钱不太够```，其中user_name代表用户名。
		2.  结束

