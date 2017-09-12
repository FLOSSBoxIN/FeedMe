# Mobilizer and full text download
Some RSS feed article just provides summary, not full text. This reading experience is not friendly. FeedMe offers some mobilizers for full download. Now support `FeedMe`，`Mercury` and `Google Web Light`. `FeedMe` is built-in mobilizer of FeedMe，the other two are third party Mobilizer services.

In FeedMe, there are two cases where mobilizer is required.
1. download when sync
2. downlaod when reading

You can find these 2 settings below (NAV side - Subscription - category/feed):

<img src="https://github.com/seazon/FeedMe/blob/master/doc/en/imgs/mobilizer_1.png" width="25%" height="25%" />

Many users asked why the third party mobilizer was set, but the article was still downloaded using FeedMe mobilizer?
Because the third party mobilizer in order to ensure the availability of its services, generally limit the frequency of calls. If the call is too fast or too many times, they will stop the service. Due to the high download frequency when FeedMe is synchronized, it may result in third party mobilizer being unavailable. So at the time of synchronization, only the built-in mobilizer is available.

So, the mobilizer in the `feed settings` dialog is only use for download when reading.

<img src="https://github.com/seazon/FeedMe/blob/master/doc/en/imgs/mobilizer_2.png" width="25%" height="25%" />

Note : Mobilizer is removing some unimportant elements on the page (head, side and bottom of the navigation or link) and re-layout, leaving only the text part. General mobilizer get the article is calculated by algorithm, so can not guarantee 100% correct. Mature mobilizer resolution is more accurate, and built-in is worse.

# Switch feed/web view manually
Once enter article page, how can I switch feed/web view manually?

### 1. Tap feed/web link
You can tap the feed/web link at top right corner. The accent color is link, and another one is current state. 

Note: If the web page is not download yet, it will download it at the first time you tap the web link. Which mobilizer it will use? Check the `feed settings` dialog article mobilizer section.

### 2. Menu `Reload page`
`Reload page` is in actionbar overflow menu, or on actionbar if you edit it. It always downloads content from web even if you downloaded the web page before. 

### 3. Double Touch
You can set the double touch action in `Settings` - `Control` as `Toggle feed/web page` to toggle between feed/web. It's behavior just like tap feed/web link.

### 4. Auto download web page
If you enable `Download web page when reading` in `feed settings` dialog, it will automatically download the full text when open the article page which the mobilizer you set.

Note: Like tap feed/web link, it just downloads web page the first time if web page is not download. Of course, if network is NOT available, it will not do anything.

# Default view
So which page will display by default? Feed or web page?
- Show feed view by default.
- Show web view if you enable `Download web page when sync` in `feed settings` and downloaded when syncing.
- Show feed view if you enable `Download web page when sync` in `feed settings` and NOT downloaded when syncing.
- Show web view if you enable `Download web page when reading` in `feed settings` and network is available.
- Show feed view if you enable `Download web page when reading` in `feed settings` and network is NOT available.

When the article content uses for some cases, like `Share content` or play it, it is also following these rules. 
