### 描述

活动管理在看到有人申请奖金的时候，驳回奖金申请

### 角色

活动管理

### 触发

当看到私信申请的时候

### 数据输入（来源）

1. 活动管理点击“❌”驳回申请

### 数据输出（去向）

领奖失败（用户）

### 路径

1. "活动管理"点击“❌”后，“Bot”私信申请者：```很遗憾这次领不到了！下次再来吧！```

### 扩展路径

1. 1. 活动管理重复点击“❌”，“bot”回复```已经驳回申请啦！```
   2. 领奖关闭后，活动管理点击“❌”，“bot”回复```已经关了啊！```