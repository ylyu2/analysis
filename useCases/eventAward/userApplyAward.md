### 描述

用户（玩家）在活动结束后，想领取奖金，增加账户余额

### 角色

任意频道用户

### 触发

当用户看到活动管理发布了领奖通知时

### 数据输入（来源）

用户点击“🎲”reaction申请领奖

### 数据输出（去向）

领奖申请是否通过（用户）
奖金数额（用户）

### 路径

1. “玩家”点击已经添加的“🎲”reaction
2. “Bot”检查“活动管理”是否通过了领奖申请

### 扩展路径

2.  
	1. 如果活动管理已经关闭领奖
		1.  “Bot”回复```user_name，活动结束啦！去参加下个活动叭！```，其中user_name指代用户名。
		2.  结束
