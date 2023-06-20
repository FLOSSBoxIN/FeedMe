### 4.0.0-Canary-5
###### 2023-6-21
- [修复] 修复操作栏菜单显示不正确的问题。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1594359875
- [修复] 修复文章列表从其他屏幕返回时自动滚动的问题。 https://github.com/seazon/FeedMe/issues/528

### 4.0.0-Canary-4
###### 2023-6-17
- [新增] 点击文章页面的feed标题可以进入该feed的文章列表页面。 https://github.com/seazon/FeedMe/issues/523
- [优化] 更新沉浸模式。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1590289087
- [修复] 修复 Tiny Tiny RSS 无法同步到未读条目的问题。 https://github.com/seazon/FeedMe/issues/525
- [修复] 修复旋转屏幕后视频停止播放的问题。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1586380529
- [修复] 修复分享到微信崩溃的问题。 https://github.com/seazon/FeedMe/issues/522#issuecomment-1593792701

### 4.0.0-Canary-3
###### 2023-6-15
- [优化]更新中文。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1590312904
- [修复]修复文章页菜单没有更新的问题。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1589336638
- [修复]修复下拉刷新不起作用的问题。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1589351824

### 4.0.0-Canary-2
###### 2023-6-13
- [修复]文章列表中的强调背景色问题。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1586292674
- [修复]左右滑动功能名称与实际功能不匹配的问题。 https://github.com/seazon/FeedMe/issues/517#issuecomment-1587651850

# 4.0.0-Canary-1
###### 2023-6-11
#### 基于 Material You 的新界面
- 卡片扁平化，圆角化 *
- 强调色在深色模式下使用低饱和度颜色
- 启动图标支持 Material You (Android 13+)
#### 大屏适配
- 根据屏幕尺寸展示不同布局
- 键盘快捷键支持 *
#### 音频
- 支持直接流媒体播放，不需要下载
- 音频支持跳过静音
- sleep time 支持单集结束
- 支持播放搜索到的，未订阅的单集
- 移除播放界面的加星功能
- 播客下载可配置
#### 视频
- 视频支持全屏播放
#### 订阅
- 输入某些网站地址时，自动转成rss地址 *
#### 其他
- 标记已读优化
  - 长按标记所有已读时，弹出更多选项（标记一天前为已读，标记一周前为已读）
  - 长按文章除了 标记以上已读外，新增 标记以下已读
- 移除文章页图片占满宽度的特性及设置项，现在总是和文字对齐
- 优化favicon显示 *
- 文章段落目录TOC *
- 新应用内支付商品：榴莲
- 内置浏览器打开外部链接时，会有提示，并且可以记住你的选择。你也可以在设置-缓存-清除默认操作 重置。

`*` 表示功能可用，但未来版本中还会继续完善