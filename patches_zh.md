### 3.0.4
###### 2017-4-9
- 新增`显示阅读时间`选项，来控制是否在文章页显示阅读时间提示，默认为不显示。
- 更新`下拉刷新`选项，新增`隐藏已读条目并同步`。
- 现在长按列表页缩略图来标记为广告图片不会在`视觉`布局起作用。
- 现在缩略图会更快显示，但gif只会显示第一帧。
- 播放菜单加入了`向左（右）滑动`快捷手势，可以在`操纵`设置中修改。
- 文章通过TTS播放完以后会自动标记为已读。
- 修复Bazqux同步问题。

### 3.0.3
###### 2017-4-6
- 实验室新增Eink闪屏优化。
- 网页浏览器和图片浏览器现在可以在设置中指定具体的外部浏览器了。
- 特殊处理时间间隔为24小时的选项，现在它只会在凌晨同步。注意，如果凌晨时因为网络不可用而没有同步，那么它会在网络可用后开始同步。同步完会把下个同步时间设置为下个凌晨。
- 缩略图可以长按并标记为广告图片，那么下次再碰到这个图片链接，就不会下载，也不会再缩略图显示。最多添加16个图片为广告图片，如果继续添加，最早加入的广告图片将不再被认为是广告图片。
- 更新部分图标。

### 3.0.1
###### 2017-3-20
- Fixed crash issue.

# 3.0
###### 2017-3-19
- Support podcast (not support `Feedbin`) and TTS. Please read <a href="https://github.com/seazon/FeedMe/blob/master/podcast_tts.md">Podcast & TTS</a> for the detail.
- Provide reading time.
- Add `Podcast` layout, which show play or download progress.
- Add `Lab` in `Settings`, including `Hardware Acceleration`.
- Improve `Accent` color, now support more color and customize color.
