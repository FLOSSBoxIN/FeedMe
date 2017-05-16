## Mobilizer 和全文下载
有些 RSS 订阅源的文章只提供摘要，而不是全文，这样的阅读体验并不友好。FeedMe 提供了多种 Mobilizer 来进行全文下载。目前支持 `FeedMe`，`Mercury` 和 `Google Web Light` 3种。`FeedMe` 为 FeedMe 自带 Mobilizer，另外2个是第三方 Mobilizer 服务。

在 FeedMe 中，有2种情况需要用到 Mobilizer。 
1. 在手动/自动同步时使用 Mobilizer 进行全文下载；
2. 在阅读时使用 Mobilizer 进行全文下载。
你可以在下图中看到这2个设置（可以通过侧边栏-订阅-类别/订阅源到达这里）：
<img src="https://github.com/seazon/FeedMe/blob/master/doc/en/imgs/mobilizer_1.png" width="25%" height="25%" />

许多用户询问为什么设置了第三方mobilizer，但是文章还是使用feedme mobilizer下载的？
因为第三方 Mobilizer 为了保证其服务的可用性，一般都会限制调用频率。如果调用过快或者次数过多，他们就会停止服务。由于 FeedMe 同步时下载频率很高，就可能因此导致第三方 Mobilizer 不可用。所以在同步时，只有自带的 Mobilizer可用。

所以，在订阅源设置中的 Mobilizer，只适用于阅读时的下载。见下图。
<img src="https://github.com/seazon/FeedMe/blob/master/doc/en/imgs/mobilizer_2.png" width="25%" height="25%" />

注：Mobilizer：去除网页上一些不重要的元素（头部，侧边及底部的导航或者链接）并重新排版，仅保留正文部分。一般 Mobilizer 得到的文章是由程序算法计算解析得出的，所以不能保证百分百的正确。成熟的Mobilizer 在正确性上会做的更好，而自带的会差一些。