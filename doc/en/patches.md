### 3.7.1
###### 2018-5-24
- [fix] Fixed crash issue.

# 3.7
###### 2018-5-23
- [new] Support share to WeChat Moments, enable in `Settings` - `Integrations`.
- [optimize] New option `Playback Speed` in `Setting` - `Audio`, disable this if TTS not work.
- [fix] Fixed some devices can't install from Play store.
- [fix] Fixed missing spaces between words in article page.
- [fix] Fixed missing subject when sharing email in some cases.

# 3.6
###### 2018-4-28
- [new] Only for supporters: Create custom launcher icon in `Setting` - `About`.
- [optimize] New optioin in `Setting` - `Interface`: Always show the NAV side when the screen is wide enough.
- [fix] Fixed cache number replacement issue.
- [fix] Fixed "open url failed" issue.
- [fix] Fixed other issues.

### 3.5.9
###### 2018-4-21
- [ATTENTION] Requests CAMERA and SHORTCUT permission to support new shortcut feature, but not available in this version.
- [fix] Fixed sync button and item count not show in NAV side on small phone.

### 3.5.8
###### 2018-4-12
- [new] Highlights NAV side item for current list.
- [new] Play page adds star menu.
- [fix] Fixed a problem where the title of the article list did not change when switched NAV side item.
- [fix] Fixed a problem of missing temporary tags.

### 3.5.7
###### 2018-4-4
- [new] When the screen width exceeds 640dp, the first screen displays both article list and the sidebar. (Android 7.1+ devices with virtual navigation bar will have display problems when rotating horizontal screen clockwise)
- [new] Support Bluetooth headset (play and stop).
- [new] `Image Browser` Add `Disable` option.
- [new] Feedbin supports self-hosted.
- [optimize] Pull down refresh always synchronizes the current list, not whole. If the current list is `all items`, it is similar to the overall synchronization.
- [optimize] Optimize the FreshRSS login experience and automatically complete the API address.
- [optimize] Optimize one-tap sharing to Todoist in article page.
- [optimize] `Temporary tag` limit raised to 5.
- [fix] Fixed false navigation position determination on Android 7.1+ devices.
- [fix] Fixed the problem that login information is not recorded when logging in for the first time (problems arise from 3.5.6).
- [fix] Fixed `Synchronous Mode` is set to `All`, but with certain feeds disabled, the number of syncs is abnormally wrong.
- [fix] Fixed the issue where FreshRSS only syncs 100 items (problems arise from 3.5.6).
- [fix] Fixed issue with using TTS playback exceptions in certain situations.

### 3.5.6
###### 2018-3-14
- [ATTENTION] Due to changes in the multi-account feature, downloaded images will not be visible after updating to the new version. If need, clear the cache and download it again.
- [optimize] Services(Feedbin, FreshRSS) that do not support feeds/categories synchronization can't modify `Sync Mode` now. `Chinese Mode` is also the same. `Sync Mode` is fixed to `All`.
- [optimize] Tiny Tiny RSS now support auth_remote.
- [fix] Fixed too many articles marked as read when enable `Auto mark read`
- [fix] Fixed FeedMe mobilizer parsing webpage garbled.
- [fix] Keyword filtering now ignores case.
- [fix] Fixed other issues.
- [other] Changes related to multi-account feature.

### 3.5.5
###### 2018-2-24
- [optimize] If there is a notification during audio playback, the playback will not be paused, but the volume will be reduced.
- [optimize] Download process shows the number of downloaded images.
- [fix] Fixed for `Json parse error` when Feedly sync.
- [fix] Fixed synchronization stuck issue of Tiny Tiny RSS when pull to refresh.
- [fix] Fixed TTS 2 word read into a word problem.
- [fix] Fixed a problem with untranslated text of list summary.
- [other] Call sync service via 3rd party app.
``` java
Intent intent = new Intent();
intent.setClassName("com.seazon.feedme", "com.seazon.feedme.service.sync.SyncService");
intent.putExtra("auto", false);
intent.putExtra("type", syncTypes);
activity.startService(intent);

// syncTypes is following (add value to do more than one action):
public static int SYNC_TO_SERVER = 1;
public static int SYNC_UNREAD_FROM_SERVER = 2;
public static int SYNC_STARRED_FROM_SERVER = 4;
public static int SYNC_DELETE_READ = 16;
public static int SYNC_DOWNLOAD_IMAGE_AND_WEB_PAGE = 32;
public static int SYNC_DOWNLOAD_PODCAST = 256;
```

### 3.5.4
###### 2018-2-8
- [new] Support FreshRSS, a self-hosted RSS service like Tiny Tiny RSS. Site: https://freshrss.org/.
- [optimize] Now thumbnails can display even if not downloaded when syncing.
- [fix] Fixed synchronization stuck issue of Tiny Tiny RSS.
- [fix] Fixed crash issue when tap subscribe menu.
- [fix] Fixed other issues.

### 3.5.3
###### 2018-1-29
- [optimize] Share link to FeedMe to subscribe. Or copy link to system clipboard, and fill automatically when click `Add subscription` menu.
- [optimize] Update French, German, Spanish, Russian, Italian, Czech, Portuguese (Brazil).
- [fix] Fixed auth failed to Feedly via Evernote.
- [fix] Fixed can't download images in some case.
- [fix] Fixed duplicate menu issue.
- [fix] Fixed other issues.
- [other] Add in-app goods: Cherry.

### 3.5.2
###### 2018-1-16
- [optimize] Update Chinese Traditional.
- [fix] Fixed Tiny Tiny RSS can only fetch 100 unread issue.
- [fix] Fixed article page can't show images after downloaded.
- [fix] Fixed pull-down refresh synchronization could not mark server-read articles as read.

### 3.5.1
###### 2018-1-12
- [new] Add new `Favorites` notification besides `Sync` and `Play`, for showing the unread info of `temporary tag`. And now you can set `show notification if new items in` in feed setting dialog. If the setted feeds have new items, also will show info in `Favorites` notification.
- [new] Support Android 8.0 notification channel. You can set different ringtone or other settings in system notification setting.
- [optimize] Now `temporary tag` show unread item count.
- [optimize] Star and unread indicator move to left side. Reading time is also affected by the `Settings` - `Interface` - `Showing Reading Time`.
- [fix] Fixed auto showing `Play` notification in some case.
- [fix] Fixed crash issue when enable `Eink Improvement`
- [fix] Fixed issues of Tiny Tiny RSS.
- [fix] Fixed images do not display even download progress bar gone in article page.

# 3.5
###### 2017-12-06
- [new] Support Tiny Tiny RSS. IMPORTANT: Go to your TTRSS web site preferences and enable "Enable API access", click "save  configuration" button and then login in FeedMe.
- [new] `Temporary tag`: Show all items which title contains keyword in one place. You can create and access it in NAV side, just like a feed. Max temporary tag count: 3.
- [new] Batch export images: If you subscribe some feed which contains a lot of images, you need to download one by one before. But now you can download all images of one feed/category one-time. The download path is same to single downloading image.Once finished, the unread articles will be marked as read if unread, and read and synced articles will be deleted.
- [optimize] Now you can hide your RSS account info via tap RSS type label which above your account name.
- [optimize] Now built-in browser is always open built-in browser, not Chrome custom tab or others.

### 3.4.3
###### 2017-11-29
- [fix] Fixed does not download images and web pages when sync in some cases.

### 3.4.2
###### 2017-11-20
- [fix] Fixed sync interval can't change issue if language is German.

### 3.4.1
###### 2017-11-16
- [optimize] Upadte German, Spanish, Portuguese (Brazil), Korean, Russian, French, Hungarian.
- [fix] Fixed some traffic settings does not work issue.
- [fix] Fixed article page can't hide action bar when scrolling issue.

# 3.4
###### 2017-11-13
- [new] Reorganize the `sync` setting. Now you can set all Wi-Fi only options in `Traffic`. The global feed settings in `Advanced`.
- [optimize] Show RSS service and account in NAV side.
- [fix] Now svg images can be displayed correctly.
- [fix] Sensitive scrolling in immersive mode.
- [fix] The bottom action bar displayed incorrectly in some cases.
- [fix] The uninstalled one-tap sharing menu can't remove from action bar.

### 3.3.2
###### 2017-10-11
- [optimize] Improve one-tap sharing system share. Now no need to reload the menus.
- [fix] Fixed DashClock issue.

### 3.3.1
###### 2017-9-15
- [fix] Fixed crash issue.

# 3.3
###### 2017-9-14
- [new] Support add system share in article page menu, then one-tap to share to your frequently-used app. (enable share in `Setting` - `Integrations`, and then you can find it in article page menus. Now maybe you need reload the menus to show it.)
- [new] Support custom notifications.
- [new] Support play video directly in the article page (add `Video Preview` in `Lab`).
- [optimize] Support horizontal display in play page.
- [optimize] Audio won't automatically downloaded after audio is disabled.
- [optimize] Some other small optimization.
- [fix] Fixed filtering does not filter for certain keyword issues.
- [fix] Fixed FeedMe Mobilizer issue in some case.

### 3.2.1
###### 2017-6-17
- [fix]Fixed Feedly login with Google auth error.
- [fix]Adapt to ultra-wide mobile phone, like S8.
- [fix]Mark item as read when open it in browser directly.

# 3.2
###### 2017-6-12
- [new]Now you can play the whole list with the new `play list` menu. (this option will clear the play list first, and the max is 100 articles.)
- [new]Support auto download podcast audio file while syncing. (download 60 minutes at least.)
- [new]Support playback speed.
- [new]Support forward/replay, and you can set time in settings.
- [new]Support play menus in article page.
- [new]Add `enable audio` option, for disable audio feature for some people who don't need this.
- [new]Add `Open in browser` option in `Settings` - `Interface`, for open item in browser directly.
- [optimize]Add `Reset` button in menu edit dialog.
- [optimize]`Card` layout supports hide summary.
- [optimize]Optimize play feature and display.
- [optimize]Add `connection close` option.
- [fix]Fixed order of starred items issue.

### 3.1.3
###### 2017-6-8
- [fix]Fixed read items back to unread issue.

### 3.1.2
###### 2017-5-20
- [optimize]Now single tap to keep unread in article page, not twice. Update the `keep unread` icon.
- [optimize]Tap feed url to copy it in feed setting page.
- [optimize]Add playback control label for TalkBack.
- [optimize]Add `Thumbnail` switch in `Lab` setting. (Just for testing)
- [fix]Fixed can't login Inoreader with Google account.
- [fix]Fixed article hard to read when enable `Eink Improvement`.

### 3.1.1
###### 2017-5-9
- [optimize]Optimize ignored thumbnail list, the same picture won't add to list.
- [optimize]Back button to exit app will hide the read items.
- [optimize]Downloading failed pictures due to network timeout will continue to be attempted at the next time.
- [fix]Fixed Bazqux issue, and improve the authentication expiration prompt of re-login tips.
- [fix]If enable split action bar, the FAB menu does not show when horizontal screen.

# 3.1
###### 2017-4-28
- [new]Support media button on headset.
- [new]Support sleep timer(on play screen).
- [new]Add feed states(`Settings` - `About`), for better understanding of feeds.
  - Show 2 values of each feed:
    - Interest value `read + star * 2`: the higher the value, the more articles you see in this feed, the more interested you are.
    - Read percent `read / ( read + glance )`: the higher the percent, the more you are interested in this feed. The percent >= 90% will be displayed frist.
  - Tap feed to show all 5 value:
    - fetch: synced articles.
    - filter: filtered articles.
    - glance: use `mark previous read` or `mark all read`.
    - read: read in article page.
    - star: starred articles.
  - Filter menu to choose scope(`today`, `this week`, `this month`, `whole`), default is `today`.
- [new]Support Chrome custom tabs.
- [optimize]Improve layout. Remove `summary` layout. Now when you select `list` layout, you can set show thumbnail/summary or not.
- [optimize]Now you can change TTS, but need restart app.
- [optimize]Change mark read time:
  - Before: enter article and mark it read. Now: leave article and mark it read.
  - Before: swipe A to B and mark B read. Now: swipe A to B and mark A read.
- [optimize]Remove Embedly mobilizer.
- [optimize]Update Spanish, Dutch, French, German, Korean, Portuguese (Brazil).
- [fix]Fixed hide thumbnail issue. You can add max 32 thumbnails. If continue add, remove the first set thumbnail.
- [fix]Fixed default browser issue, add `built-in` option. Now `default` means system default browser. If the system default browser does not set, show select dialog.

### 3.0.4
###### 2017-4-9
- Add an option `Show Reading Time` in `Interface` setting to show reading time in article page, default is false.
- Update `Pull to Refresh` option in `Control`, add a new item `Hide read items and sync`.
- Now long press on article list item won't work in `Visioin` layout.
- Now thumbnails load faster, and gif just shows first frame.
- Play menus add to `Swipe Left(Right) to Right(Left)` options.
- Auto mark item as read when read article via TTS.
- Fixed Bazqux sync issue.

### 3.0.3
###### 2017-4-6
- Add `Eink Improvement` in `Lab`.
- Now you can set specific browser for browser and image browser.
- Now `24 hours` of `Auto Sync` is a special processing interval option, it will only sync in midnight. Note that if it does not sync in midnight, it will be synchronized when the network is available. And next synchronization time is the next midnight.
- Thumbnails can be long press and marked as AD images, then this picture will no longer be a thumbnail. You can add up to 16 images for the AD image. If you continue to add, the first AD image will no longer be considered an AD image.
- Update some icons.

### 3.0.1
###### 2017-3-20
- Fixed crash issue.

# 3.0
###### 2017-3-19
- Support podcast (not support `Feedbin`) and TTS. Please read <a href="https://github.com/seazon/FeedMe/blob/master/doc/en/podcast_tts.md">Podcast & TTS</a> for the detail.
- Provide reading time.
- Add `Podcast` layout, which show play or download progress.
- Add `Lab` in `Settings`, including `Hardware Acceleration`.
- Improve `Accent` color, now support more color and customize color.
