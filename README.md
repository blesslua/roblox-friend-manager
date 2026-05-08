# Roblox Friend Manager

A free Chrome extension to bulk manage your Roblox friends, requests, followers, and following from one clean panel.

Built with Roblox's native dark theme so it feels like part of the site.

## Features

- **Bulk unfriend** select many friends at once and unfriend them in one go
- **Bulk decline** clear out friend requests fast
- **Bulk accept** accept multiple friend requests at once
- **Bulk remove followers** uses block then unblock to remove followers cleanly
- **Bulk unfollow** clear your following list quickly
- **Drag to select** click and drag your mouse over users to mass select them
- **Search filter** find users by username or display name instantly
- **Rate limit handling** auto retries when Roblox rate limits you so you dont have to babysit it
- **No account info collected** uses your existing browser session everything stays local

## Install

1. Download the latest `roblox-friend-manager.zip` from the [Releases](../../releases) page
2. Extract the zip you should get a folder called `roblox-friend-manager`
3. Open `chrome://extensions` in Chrome, Edge, Brave, or Opera
4. Turn on **Developer mode** (top right toggle)
5. Click **Load unpacked** and select the extracted `roblox-friend-manager` folder (the one containing `manifest.json`)
6. Make sure youre signed into [roblox.com](https://www.roblox.com) in the same browser
7. Click the extension icon in your toolbar to open the panel

If the extension icon isnt visible click the puzzle piece icon in your toolbar and pin it.

## How to use

- Click any tab to view that list (Friends, Requests, Followers, Following)
- Click users to select them, or hold and drag to mass select
- Hit the action button to bulk remove
- Hold Alt while dragging to deselect a range

## How it works

The extension uses Roblox's official web API endpoints with your existing browser session cookies. CSRF tokens are handled automatically. There is no external server, no proxy, no credentials stored, and no data collected.

For the followers tab, since Roblox has no direct "remove follower" endpoint, the extension blocks then immediately unblocks each user which removes them from your followers list. Your block list stays empty after.

## Disclaimer

This extension is unofficial and not affiliated with Roblox Corporation. Use it at your own discretion and follow Roblox's [Terms of Use](https://en.help.roblox.com/hc/en-us/articles/115004647846-Roblox-Terms-of-Use).

## License

MIT
