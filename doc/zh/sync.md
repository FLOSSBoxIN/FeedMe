# 使用按钮或者手势进行同步

# 高级同步对话框

# 自动同步设置

# 同步未读条数
同步未读条数在`设置`-`缓存`-`未读条目`设置。如果设置了500条，而服务端未读条数大于等于500条，那么每次同步会下载最新的500条。如果小于500条，那就全部下载。

# 同步模式
提供多种同步模式来满足不同需求。

## 整体
仅根据文章发布时间进行同步。整体下载逻辑及例子：
（下载250条未读，按照时间倒序排序）
下载100条
下载100条
下载50条
这种方式是最快的下载方式，但是不能禁止下载某些`订阅源`或者`类别`。
注意：如果启用`中国模式`，则强制使用`整体`模式。

## 类别
按`类别`进行同步。按`类别`下载逻辑及例子：
（下载90条未读，90条未读分别属于3个`类别`，那么会先把3个`类别`按照未读数排序，优先拉取未读数少的`类别`。比如类别A有10条未读，类别B有30条未读，类别C有50条未读）
下载类别A 10条
下载类别B 20条
下载类别C 20条
下载类别B 10条
下载类别C 20条
下载类别C 10条

可以禁止`类别`同步，但是不能禁止`订阅源`同步。
注意，按`类别`同步无法同步到未分类的订阅源的文章。


## 订阅源
按照`订阅源`进行同步。按`订阅源`下载逻辑及例子：
（下载90条未读，90条未读分别属于3个`订阅源`，那么会先把3个`订阅源`按照未读数排序，优先拉取未读数少的`订阅源`。比如订阅源A有10条未读，订阅源B有30条未读，订阅源C有50条未读）
下载订阅源A 10条
下载订阅源B 20条
下载订阅源C 20条
下载订阅源B 10条
下载订阅源C 20条
下载订阅源C 10条

可以禁止`订阅源`同步，但是不能禁止`类别`同步。