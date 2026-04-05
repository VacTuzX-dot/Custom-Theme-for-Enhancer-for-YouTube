# Custom Theme for Enhancer for YouTube

Custom CSS themes for YouTube, made for [Enhancer for YouTube](https://www.mrfdev.com/enhancer-for-youtube).

## Theme

| Theme | File | Notes |
| --- | --- | --- |
| Amethyst | [`themes/AmethystTheme.css`](./themes/AmethystTheme.css) | Purple glass theme with light mode and dark mode support |

## What It Changes

- Sidebar and masthead
- Search bar and dropdowns
- Player, watch page, and comments
- Menus, dialogs, and notifications
- Channel page, live chat, and miniplayer

## Install

1. Install Enhancer for YouTube.
2. Open `Settings -> Custom CSS`.
3. Paste the content of [`themes/AmethystTheme.css`](./themes/AmethystTheme.css).
4. Click `Save`.
5. Reload YouTube.

### Store Links

| Browser | Link |
| --- | --- |
| Chrome | [Chrome Web Store](https://chrome.google.com/webstore/detail/enhancer-for-youtube/ponfpcnoihfmfllpaingbgckeeldkhle) |
| Firefox | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/enhancer-for-youtube/) |
| Edge | [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/enhancer-for-youtube/dlgfaleeejmphhnemjgiaekdbonkagkd) |

## Use `@import` Instead of Pasting Full CSS

If the full file is too long for the editor, use this:

```css
@import url("https://cdn.jsdelivr.net/gh/VacTuzX-dot/Custom-Theme-for-Enhancer-for-YouTube@main/themes/AmethystTheme.css");
```

> **Note:** Do **not** paste this line inside `AmethystTheme.css` itself — that causes an infinite import loop. Paste it only into Enhancer for YouTube's **Custom CSS** box.

### Why updates aren't instant (jsDelivr caching)

jsDelivr caches the `@main` branch for up to **24 hours**. After pushing new commits, the CDN may still serve the old version.

**To force an immediate update after pushing:**

1. Open this URL in your browser:  
   [`https://purge.jsdelivr.net/gh/VacTuzX-dot/Custom-Theme-for-Enhancer-for-YouTube@main/themes/AmethystTheme.css`](https://purge.jsdelivr.net/gh/VacTuzX-dot/Custom-Theme-for-Enhancer-for-YouTube@main/themes/AmethystTheme.css)
2. Wait a few seconds for the purge to complete.
3. Reload YouTube — the new styles will apply immediately.

Other notes:

- If you want a pinned version that never changes, replace `@main` with a specific commit hash.
- If `@import` does not load in your browser, paste the full CSS file instead.

## Customize

Edit the variables at the top of [`themes/AmethystTheme.css`](./themes/AmethystTheme.css).

- `:root` contains shared colors.
- `html[dark], [dark]` contains dark mode colors.
- `html:not([dark])` contains light mode colors.

Start with these groups:

- `--yt-purple-primary`, `--yt-purple-accent`
- `--yt-base-*`
- `--yt-surface-*`
- `--yt-purple-text`

## Requirements

- Enhancer for YouTube `3.0.17` or later
- Hardware acceleration enabled if you want blur effects to look correct

## Notes

- The theme supports both YouTube light mode and dark mode.
- YouTube changes its HTML and class names often. Some selectors may need updates later.

## Contributing

1. Copy a file from [`themes/`](./themes/).
2. Rename it.
3. Update the color variables.
4. Add it to the theme table above.
5. Open a pull request.

## License

[MIT](./LICENSE)
