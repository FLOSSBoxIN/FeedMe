# Use button or gesture to synchronize

# Sync action

# Auto sync settings

# Unread count of synchronization
The number of unread items to synchronize is set in `Settings`-`Cache`-`Reading List`. If 500 are set, and the number of unread items on the server side is greater than 500, the latest 500 will be downloaded for each synchronization. If it is less than 500, download all of them.

# Sync mode
Provide multiple synchronization modes to meet different needs.

## All
Synchronize only based on the publish time of the article.

Example:
- Download latest 250 unread
- Download 100
- Download 100
- Download 50

This method is the fastest way to download, but you cannot exclude certain `feeds` or `categories`.

Note: If the `China Mode` is enabled, the `All` mode is mandatory.

## Categories
Sync by category

Example:
- 90 unread items wait to download, these 90 unread items belong to 3 `categories`
- sort these `categories`, fewer unread count has higher priority to sync.
- category A has 10 unread items, category B has 30 unread, category C has 50 unread
- Download category A 10
- Download category B 20
- Download category C 20
- Download category B 10
- Download category C 20
- Download category C 10

Can exclude certain categories, but can't exclude feeds.

Note that synchronization by `category` cannot be synchronized to articles from uncategorized feeds.

## Feeds
Sync by feed

Example:
- 90 unread items wait to download, these 90 unread items belong to 3 `feeds`
- sort these `feeds`, fewer unread count has higher priority to sync.
- feeds A has 10 unread, feed B has 30 unread, and feed C has 50 unread
- Download feed A 10
- Download feed B 20
- Download feed C 20
- Download feed B 10
- Download feed C 20
- Download feed C 10

Can exclude certain feeds, but can't exclude categories.