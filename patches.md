# 3.1
###### 2017-4-28
- [new]Support media button on headset.
- [new]Support sleep timer(on play screen).
- [new]Add feed states(`Settings` - `About`), for better understanding of feeds.
  - Show 2 values of each feed:
    - Interest value `read + star * 2`: the higher the value, the more articles you see in this feed, the more interested you are.
    - Read percent `read / ( read + glance )`: the higher the percent, the more you are interested in this feed. The percent >= 90% will be displayed frist.
  - Click feed to show all 5 value:
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
- Now long tap on article list item won't work in `Visioin` layout.
- Now thumbnails load faster, and gif just shows first frame.
- Play menus add to `Swipe Left(Right) to Right(Left)` options.
- Auto mark item as read when read article via TTS.
- Fixed Bazqux sync issue.

### 3.0.3
###### 2017-4-6
- Add `Eink Improvement` in `Lab`.
- Now you can set specific browser for browser and image browser.
- Now `24 hours` of `Auto Sync` is a special processing interval option, it will only sync in midnight. Note that if it does not sync in midnight, it will be synchronized when the network is available. And next synchronization time is the next midnight.
- Thumbnails can be long pressed and marked as AD images, then this picture will no longer be a thumbnail. You can add up to 16 images for the AD image. If you continue to add, the first AD image will no longer be considered an AD image.
- Update some icons.

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
