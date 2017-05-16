## Mobilizer and full text download
Some RSS feed article just provides summary, not full text. This reading experience is not friendly. FeedMe offers some mobilizers for full download. Now support `FeedMe`，`Mercury` and `Google Web Light`. `FeedMe` is built-in mobilizer of FeedMe，the other two are third party Mobilizer services.

In FeedMe, there are two cases where mobilizer is required.
1. download when sync
2. downlaod when reading
You can find these 2 settings below (NAV side - Subscription - category/feed):
<img src="https://github.com/seazon/FeedMe/blob/master/doc/en/imgs/mobilizer_1.png" width="25%" height="25%" />

Many users asked why the third party mobilizer was set, but the article was still downloaded using FeedMe mobilizer?
Because the third party mobilizer in order to ensure the availability of its services, generally limit the frequency of calls. If the call is too fast or too many times, they will stop the service. Due to the high download frequency when FeedMe is synchronized, it may result in third party mobilizer being unavailable. So at the time of synchronization, only the built-in mobilizer is available.

So, the mobilizer in the feed settings is only use for download when reading.
<img src="https://github.com/seazon/FeedMe/blob/master/doc/en/imgs/mobilizer_2.png" width="25%" height="25%" />

Note : Mobilizer is removing some unimportant elements on the page (head, side and bottom of the navigation or link) and re-layout, leaving only the text part. General mobilizer get the article is calculated by algorithm, so can not guarantee 100% correct. Mature mobilizer resolution is more accurate, and built-in is worse.
