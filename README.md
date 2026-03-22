<div align="center">

<br/>

```
 ██╗░░░██╗████████╗  ████████╗██╗░░██╗███████╗███╗░░░███╗███████╗░██████╗
 ╚██╗░██╔╝╚══██╔══╝  ╚══██╔══╝██║░░██║██╔════╝████╗░████║██╔════╝██╔════╝
 ░╚████╔╝░░░░██║░░░  ░░░██║░░░███████║█████╗░░██╔████╔██║█████╗░░╚█████╗░
 ░░╚██╔╝░░░░░██║░░░  ░░░██║░░░██╔══██║██╔══╝░░██║╚██╔╝██║██╔══╝░░░╚═══██╗
 ░░░██║░░░░░░██║░░░  ░░░██║░░░██║░░██║███████╗██║░╚═╝░██║███████╗██████╔╝
 ░░░╚═╝░░░░░░╚═╝░░░  ░░░╚═╝░░░╚═╝░░╚═╝╚══════╝╚═╝░░░░╚═╝╚══════╝╚═════╝░
```

**Custom CSS theme collection for YouTube**  
*Built for [Enhancer for YouTube](https://www.mrfdev.com/enhancer-for-youtube) · free & open source*

<br/>

![Version](https://img.shields.io/badge/version-1.0.0-555?style=flat-square&labelColor=111)
![Enhancer](https://img.shields.io/badge/Enhancer%20for%20YouTube-3.0.17+-555?style=flat-square&labelColor=111)
![License](https://img.shields.io/badge/license-MIT-555?style=flat-square&labelColor=111)
![Dark Mode](https://img.shields.io/badge/dark%20mode-required-555?style=flat-square&labelColor=111)

<br/>

</div>

---

## // Overview

**YT Themes** is an open collection of custom CSS themes for YouTube, designed to work with the [Enhancer for YouTube](https://www.mrfdev.com/enhancer-for-youtube) browser extension.

Each theme replaces YouTube's default dark UI with a cohesive color palette — using glassmorphism-style surfaces, blur backdrops, rounded corners, and consistent tinted borders across the entire interface.

Every theme covers the same set of components: masthead, sidebar, player, watch page, comments, feed, menus, channel pages, live chat, and miniplayer. Pick one, paste it in, done.

---

## ◈ Available Themes

| Theme | Palette | File |
|-------|---------|------|
| Amethyst | Deep purple — `#0d0618` → `#A855F7` | [`themes/AmethystTheme.css`](./AmethystTheme.css) |
| _(more coming)_ | — | — |

> Want to contribute a theme? See [Contributing](#-contributing) below.

---

## ▸ What Each Theme Covers

All themes apply consistent styling across these sections:

<details>
<summary><b>UI & Navigation</b></summary>

- Frosted glass masthead with accent border
- Auto-hide sidebar with blur backdrop
- Search bar with accent focus ring
- Prediction dropdown with glass surface
- Voice search button tinted

</details>

<details>
<summary><b>Player & Controls</b></summary>

- Rounded video container (13px radius)
- Progress bar tooltip with glass background
- Quality menu with hover states
- Endscreen cards (video, playlist, channel, website)
- Captions with frosted pill background
- SponsorBlock notice styled to match
- Info cards and teaser overlays

</details>

<details>
<summary><b>Watch Page Metadata</b></summary>

- Description card with accent border
- Action buttons (like, share, save) tinted
- Chapter markers with accent timestamps
- Gaming info card
- Merch shelf and rich header cards

</details>

<details>
<summary><b>Comments</b></summary>

- Author name pill chip with accent background
- Submit button uses primary accent color
- Emoji picker with glass surface
- Creator heart in accent color

</details>

<details>
<summary><b>Feed & Thumbnails</b></summary>

- Rounded thumbnails (12px)
- Duration badge with dark base + blur
- Feed filter chips with accent tint
- Post cards with subtle surface color
- Show more button styled

</details>

<details>
<summary><b>Menus, Popups & Dialogs</b></summary>

- All dropdowns: glass surface + accent border
- Notification center
- Account menu
- Save to playlist dialog
- Share panel
- Context menus

</details>

<details>
<summary><b>Channel Page</b></summary>

- Header backdrop blur with accent tint
- Tab bar with glass surface
- Avatar rounded corners throughout

</details>

<details>
<summary><b>Live Chat & Miniplayer</b></summary>

- Chat header with accent tint
- Input area transparent
- Miniplayer with accent border + blur

</details>

---

## ↓ Installation

**1. Install the extension**

| Browser | Link |
|---------|------|
| Chrome | [Chrome Web Store](https://chrome.google.com/webstore/detail/enhancer-for-youtube/ponfpcnoihfmfllpaingbgckeeldkhle) |
| Firefox | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/enhancer-for-youtube/) |
| Edge | [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/enhancer-for-youtube/dlgfaleeejmphhnemjgiaekdbonkagkd) |

**2. Get a theme file**

```bash
# Clone the whole repo
git clone https://github.com/YOUR_USERNAME/yt-themes.git

# Or grab a single theme directly
curl -O https://raw.githubusercontent.com/YOUR_USERNAME/yt-themes/main/themes/amethyst.css
```

**3. Paste into Enhancer**

```
Enhancer for YouTube → [ Settings ] → Custom CSS → paste contents → Save
```

**4. Reload YouTube** — done.

---

## ~ Customization

Every theme is built around a small set of CSS variables at the top of the file. Fork any theme, swap the values, and you have a completely new palette — no other changes needed.

```css
:root {
  /* -- base backgrounds -- */
  --yt-theme-base:    #0d0618;    /* deepest bg */
  --yt-theme-surface: #2d106080;  /* panels, drawers */
  --yt-theme-mid:     #4c1d9566;  /* cards, chips */

  /* -- accents -- */
  --yt-theme-primary: #7C3AED;    /* buttons, borders */
  --yt-theme-accent:  #A855F7;    /* hover states */
  --yt-theme-hi:      #C084FC;    /* highlights */

  /* -- text -- */
  --yt-theme-text:    #ede9fe;    /* text on colored surfaces */
}
```

Change those 7 values — everything else in the file references these variables. No hunting through hundreds of lines.

---

## + Contributing

Contributions are welcome. To add a new theme:

1. Fork this repo
2. Copy any existing file from `themes/` as a starting point
3. Rename it to your theme (e.g. `themes/rose.css`)
4. Update the `:root` variables with your palette
5. Add a row to the **Available Themes** table in this README
6. Open a pull request

No strict rules on palette style — dark, light, monochrome, neon, muted, whatever works. The only requirement is that the file covers all the same CSS sections as existing themes so coverage stays consistent.

---

## § Requirements

- **Enhancer for YouTube** `3.0.17` or later
- YouTube **dark mode** enabled (Settings → Appearance → Dark theme)
- Browser hardware acceleration **on** — required for `backdrop-filter` blur effects
- Tested on **Chrome 120+** / **Firefox 121+**

---

## ! Notes

> **Sidebar auto-hide** — the CSS handles visuals only. The actual hide/show behavior requires the corresponding JavaScript snippet to be enabled inside Enhancer for YouTube's settings separately.

> **backdrop-filter** — if panels appear solid instead of frosted, check that GPU acceleration is enabled in `chrome://settings` → System.

> **YouTube UI updates** — YouTube frequently changes its internal class names. If something breaks after an update, open an issue and a fix will be pushed.

---

## * License

MIT — use it, fork it, sell it, do whatever. Credit is appreciated but not required.

---

<div align="center">

made with ♥ in chiang mai

</div>
