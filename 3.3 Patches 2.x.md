<h6>2.6.2 2017-3-2</h6>
<fmi>- Support dir tag of HTML.</fmi>
<fmi>- Add "Mark Read Action" option in Interface setting.</fmi>
<fmu>- Improve feed manager dialog.</fmu>
<fmu>- Update French, Dutch, Hungarian, German, Spanish, Russian, Chinese Traditional, Czech.</fmu>
<fmd>- Fixed custom action bar error icons and text issues.</fmd>
<fmd>- Fixed incomplete count of article page issue.</fmd>
<fmd>- Fixed repeat loadig issue of built-in browser.</fmd>

<h6>2.6.1 2017-1-23</h6>
<fmi>- Add new option to Pull to Refresh: Hide read items.</fmi>
<fmi>- Mark all read now auto open the next category/feed. If current is last, open NAV side.</fmi>
<fmi>- Support one key to delete for input field.</fmi>
<fmi>- Now you can add feed to Feedbin.(Title and category in subscription dialog not work, and not support unsubscribe)</fmi>
<fmu>- Update Korean, Hungarian, Portuguese (Brazil), Romanian.</fmu>
<fmd>- Fixed share content issue.</fmd>

<h1>2.6 2016-12-18</h1>
<fmi>- Support TeslaUnread. And use these codes to get unread count and sync time for developers:</fmi>
<fmi><pre>
    Intent batteryIntent = context.registerReceiver(null, new IntentFilter("com.seazon.feedme.ACTION_UNREAD_COUNT"));
    int unreadCount = batteryIntent.getIntExtra("UNREAD_COUNT", -1);
    long syncTime = batteryIntent.getLongExtra("SYNC_TIME", -1);
</pre></fmi>
<fmi>- Improve E-Ink experience. Some optimizations are only effective for E-Ink theme.</fmi>
<fmi>- Build-in save page function, including images. You can save page via "Share content" and choose "Save html".</fmi>
<fmi>- Add "Indent" option in article view dialog.</fmi>
<fmu>- Rename widget.</fmu>
<fmu>- Remove Readability service.</fmu>
<fmd>- Fixed audio tag issue.</fmd>
<fmd>- Other bugfixes and improvements.</fmd>

<h6>2.5.6 2016-11-27</h6>
<fmi>- The Readability Parser API will shut down December 10, 2016. And now FeedMe supports Mercury mobilizer. Another mobilizer Google web light seems to have some problems in FeedMe.</fmi>
<fmi>- New setting Interface - Navigation Bar, fix the wrong FAB or bottom bar position.</fmi>
<fmu>- Update Portuguese (Brazil).</fmu>
<fmd>- Fixed show same pictures in article. Only works on newly downloaded articles.</fmd>
<fmd>- Fixed save picture failed issue.</fmd>
<fmd>- Other bugfixes and improvements.</fmd>

<h6>2.5.5 2016-10-28</h6>
<fmi>- Support Indonesian.</fmi>
<fmu>- Update German.</fmu>
<fmu>- Align add "justify" option.</fmu>
<fmu>- Gif in item list play one time if not move.</fmu>
<fmd>- Embedly mobilizer now can shows error information correctly.</fmd>
<fmd>- Pocket mobilizer does not work anymore, removed.</fmd>
<fmc>- Update okhttp 2.3.0 -> 3.4.1.</fmc>

<h6>2.5.4 2016-9-20</h6>
<fmd>- Fixed split action bar issue.</fmd>
<fmd>- Fixed scroll bar issue.</fmd>
<fmd>- Fixed side nav header issue.</fmd>

<h6>2.5.3 2016-9-10</h6>
<fmu>- Improve immersive mode, now there are three options.</fmu>
<fmu>- Now sync notification also shows new item count.</fmu>
<fmu>- Improve checkbox style for Android 4.0.</fmu>
<fmu>- Improve switch style for Android 4.0 ~ 4.4.</fmu>
<fmd>- Fixed authentication expired issue, now a dialog will show to re-authentication.</fmd>

<h6>2.5.2 2016-8-27</h6>
<fmi>- Improve audio tag and video tag in article page. Now it displays an icon, click to open audio/video app to play.</fmi>
<fmu>- Update Spanish, Russian.</fmu>
<fmu>- Some improvements.</fmu>
<fmd>- Fixed font load issue.</fmd>
<fmd>- Fixed only sync when charging issue.</fmd>

<h6>2.5.1 2016-8-13</h6>
<fmi>- New widget.</fmi>
<fmu>- Update Spanish, Russian, German, Polish.</fmu>
<fmu>- Some improvements.</fmu>

<h1>2.5 2016-7-8</h1>
<fmi>- Now you can customize menus on actionbar and FAB(floating action button), set one FAB and some menus show if space is enough(if no space, show in overflow), set some menus always in overflow, set some menus disable, and re-order them.
adapter for all activities.</fmi>
<fmi><li>update split actionbar mode: show actionbar with menus at bottom for phone or show at side for tablet.</li></fmi>
<fmi><li>update handness option: decide FAB, side actionbar and swipe back at which side: left or right.</li></fmi>
<fmi><li>long click actionbar title to enter edit mode.</li></fmi>
<fmi><li>provide back, up and down menu for tablet, you also can use them on phone.</li></fmi>
<fmi>- Improve actionbar and animation</fmi>
<fmi><li>transparent actionbar for android 5.0+.</li></fmi>
<fmi><li>scroll up to hide actionbar and scroll down to show.</li></fmi>
<fmi><li>scroll down to the bottom to show actionbar again, if in immersive mode article page, actionbar won't show.</li></fmi>

<h6>2.4.2 2016-7-6</h6>
<fmi>- Support mute keywords(in feed manager dialog).</fmi>
<fmu>- Update Portuguese (Brazil), Romanian.</fmu>

<h6>2.4.1 2016-6-7</h6>
<fmi>- New option to disable pull to refresh in article list page.</fmi>
<fmi>- New option to open image in third party image browser.</fmi>
<fmi>- New option to save image when long press on image in article page.</fmi>
<fmu>- Improve sync issue for Android 6.0 Doze feature.</fmu>
<fmd>- Other bugfixes and improvements.</fmd>
<fmc>- Add local RSS feature, but not ready related plug-ins.</fmc>

<h1>2.4 2016-5-16</h1>
<fmi>- Add new launch mode (Settings - Interface) : Launch screen is article list, right swipe to open nav side, and back button to article list, and back again to exit.</fmi>
<fmi>- Improve subscription 1 : Now you can manager category in subscription page. Tap category to show category setting dialog.</fmi>
<fmi>- Improve subscription 2 : Layout (List, Card, etc.) is now remembered for each feed and category.</fmi>
<fmi>- Improve subscription 3 : Set different mobilizer for different feed/category.</fmi>
<fmi>- Improve subscription 4 : Set keywords for feed to filter articles. Once the keywords seted for feed, only the articles which title contains the keywords will reserved, other articles will mark as read. You can set more than one keyword for one feed, split them by ";". If you want to add a filter which need both meet two keywords or more, connect them by "+".</fmi>
<fmi>- Sync mode:</fmi>
<fmi><li>by feed : The sync mode we used before 2.4. Sync articles group by feed. You can disable sync some feeds.</li></fmi>
<fmi><li>by category : Sync articles group by category. You CAN'T sync uncategoried feeds. You can disable sync some categories, but CAN'T disable sync some feeds.</li></fmi>
<fmi><li>by all : Sync articles just order by time. The fastest way to sync. You CAN'T disable sync some feeds or categories. This is the sync mode if you enable "China Mode" before 2.4.</li></fmi>
<fmi>- Support Dutch.</fmi>
<fmu>- Improve dialog width for tablet.</fmu>
<fmd>- Fixed Feedbin button issue.</fmd>
<fmd>- Fixed list jump issue when add article to Pocket in article list page.</fmd>

<h1>2.3 2016-4-18</h1>
<fmi>- Support Feedbin.</fmi>
<fmi>- Add In-app Billing (Settings - About).</fmi>
<fmd>- Fixed margin, line-height, align setting reset issue.</fmd>

<h6>2.2.9 2016-4-11</h6>
<fmi>- New option in Feed Setting: Download web page when reading. (via Readability mobilizer)</fmi>
<fmi>- Now starred items won't download web page if this feed not enable download web page when sync.</fmi>
<fmi>- New layout：Vision.</fmi>
<fmi>- Support video tag in article page.</fmi>
<fmi>- Add margin, line-height, align in view menu of article page.</fmi>
<fmu>- Update Hungarian, Spanish.</fmu>
<fmu>- Improve image browser.</fmu>
<fmc>- Update library: android support lib:23.1.1 -> 23.3.0, glide:3.6.1 -> 3.7.0, PhotoView:1.2.2 -> 1.2.5.</fmc>

<h6>2.2.8 2016-4-7</h6>
<fmu>- Update German.</fmu>
<fmd>- Fixed a sync issue of InoReader OAuth 2. You need re-login to solve this bug.</fmd>

<h6>2.2.7 2016-3-30</h6>
<fmu>- Support Hungarian, update Spanish, Portuguese (Brazil), French, Russian, Ukrainian, Japanese.</fmu>
<fmu>- User authentication via OAuth 2.0 for InoReader.</fmu>
<fmu>- Support copy to clipboard menu when long tap in article list.</fmu>
<fmd>- Fixed a sync issue of The Older Reader.</fmd>

<h6>2.2.6 2016-3-24</h6>
<fmu>- Add open source licenses page in setting.</fmu>
<fmu>- Improve Everntoe sharing.</fmu>
<fmu>- Improve progress bar style.</fmu>
<fmu>- Improve FAB: show in left/right base on One-Hand Operation setting.</fmu>
<fmu>- Update Russian, French and Spanish.</fmu>
<fmc>- Minimum support from 2.3 to 4.0.</fmc>
<fmc>- Custom events.</fmc>

<h6>2.2.5 2016-3-13</h6>
<fmd>- Fix sync issue.</fmd>

<h6>2.2.4 2016-3-11</h6>
<fmd>- Update for InoReader user.</fmd>
<fmc>- Get more information <a href="https://plus.google.com/100365587272890955375/posts/MffXHfkUBB8">here</a></fmc>

<h6>2.2.3 2016-3-10</h6>
<fmd>- Bugfixes and improvements.</fmd>

<h6>2.2.2 2016-3-9</h6>
<fmu>- Update Spanish and Russian.</fmu>
<fmd>- Fixed crash issue while mark all read.</fmd>
<fmd>- Fixed wrong category counts issue.</fmd>
<fmd>- Other bugfixes and improvements.</fmd>

<h6>2.2.1 2016-2-28</h6>
<fmi>- New layout "Summary" which show title and summary.</fmi>
<fmu>- Now you can change font in list page via view menu.</fmu>
<fmu>- Now sync progress won't show in notification bar, but in nav side. And also will show when auto sync.</fmu>
<fmu>- Now changing theme in list page won't open drawer.</fmu>
<fmu>- Now changing theme in setting page won't reset to sync tab.</fmu>
<fmu>- Now list page uses regular font, not light font, for readability.</fmu>
<fmu>- Now alert dialog will show at bottom if enable split action bar (settings - control).</fmu>
<fmu>- Other UI improvements.</fmu>
<fmc>- No longer support Android 2.2 for network issue.</fmc>

<h1>2.2 2016-2-15</h1>
<fmi>- Support auto theme change (settings - ui). If using Light or Paper theme, auto change to Dark theme when before 6 am or after 18 pm.</fmi>
<fmi>- Add more actions for double tap in article page.</fmi>
<fmu>- Tap action bar title to back to top for list and article page.</fmu>
<fmu>- Read and unstarred item title shows a lighter color.</fmu>
<fmu>- Improve setting page.</fmu>
<fmu>- Improve theme change animation.</fmu>
<fmu>- Improve mobilizer tag.</fmu>
<fmd>- Fixed some FC issues.</fmd>
<fmc>- Improve Overdraw.</fmc>

<h6>2.1.1 2016-2-4</h6>
<fmd>Fixed sync issue occur in 2.1.0.</fmd>

<h1>2.1 2016-1-29 2016-2-4</h1>
<fmi>- Support in app search.</fmi>
<fmi>- Optimize manual synchronization.</fmi>
<fmi>- Support share to Wiz note.</fmi>
<fmi>- Add "keep unread" for swipe fast action.</fmi>
<fmu>- Optimize article page tag h1~h6.</fmu>
<fmd>- Fixed nav side group expand issue.</fmd>
<fmd>- Fixed a FeedMe mobilizer bug.</fmd>
<fmd>- Fixed subscription issue.</fmd>
<fmu>- Adjust font size of article list summary and article page title.</fmu>
<fmu>- Support android 6.0 permission.</fmu>
<fmc>- Get more information <a href="https://plus.google.com/100365587272890955375/posts/dVqaNifMSsZ">here</a></fmc>

<h6>2.0.6 2016-1-17</h6>
<fmu>- Improve FAB show again when scroll to bottom.</fmu>
<fmu>- Improve FAB hide/show via volume buttons navigation.</fmu>
<fmd>- Fixed some favicons not show issue.</fmd>
<fmd>- Fixed can't save image issue.</fmd>

<h6>2.0.5 2015-12-24</h6>
<fmd>- Fixed can't open article and FC(sometimes) issue.</fmd>

<h6>2.0.4 2015-12-23</h6>
<fmd>- Fixed can't save to Instapaper issue</fmd>
<fmd>- Fixed conflict of swipe and pull to refresh.</fmd>
<fmu>- Improve star FAB in article page</fmu>

<h6>2.0.3 2015-12-18</h6>
<fmu>- Sync menu back.</fmu>
<fmd>- Fixed FC issue on tablet.</fmd>
<fmd>- Other minor changes and bug fixes.</fmd>

<h6>2.0.2 2015-12-16</h6>
<fmu>- Optimize built-in browser.</fmu>
<fmu>- Optimize minimal view for small screen.</fmu>
<fmu>- Optimize font initialization.</fmu>
<fmc>- Remove depricated Instapaper Mobilizer.</fmc>

<h6>2.0.1 2015-11-25</h6>
<fmd>- Fix FC issue when open app in Android 6.0.</fmd>

<h1>2.0 2015-11-24</h1>
<fmi>- Pull to refresh.</fmi>
<fmi>- Selectable font.</fmi>
<fmi>- Adjustable font size in list.</fmi>
<fmi>- Card, list, minimal list view, with summary and thumbnail.</fmi>
<fmi>- Auto mark read.</fmi>
<fmi>- Material elements: ripple, float action bar.</fmi>
<fmi>- One more theme: paper.</fmi>
<fmi>- Selectable color.</fmi>
