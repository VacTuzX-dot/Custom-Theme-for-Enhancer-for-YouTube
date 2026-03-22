<div align="center">

<br/>

```
 ░█████╗░███╗░░░███╗███████╗████████╗██╗░░██╗██╗░░░██╗░██████╗████████╗
 ██╔══██╗████╗░████║██╔════╝╚══██╔══╝██║░░██║╚██╗░██╔╝██╔════╝╚══██╔══╝
 ███████║██╔████╔██║█████╗░░░░░██║░░░███████║░╚████╔╝░╚█████╗░░░░██║░░░
 ██╔══██║██║╚██╔╝██║██╔══╝░░░░░██║░░░██╔══██║░░╚██╔╝░░░╚═══██╗░░░██║░░░
 ██║░░██║██║░╚═╝░██║███████╗░░░██║░░░██║░░██║░░░██║░░░██████╔╝░░░██║░░░
 ╚═╝░░╚═╝╚═╝░░░░╚═╝╚══════╝░░░╚═╝░░░╚═╝░░╚═╝░░░╚═╝░░░╚═════╝░░░░╚═╝░░░
```

**A deep amethyst purple theme for YouTube**  
*Built for [Enhancer for YouTube](https://www.mrfdev.com/enhancer-for-youtube) extension*

<br/>

![Version](https://img.shields.io/badge/version-1.0.0-7C3AED?style=flat-square&labelColor=1a0a2e)
![Enhancer](https://img.shields.io/badge/Enhancer%20for%20YouTube-3.0.17+-A855F7?style=flat-square&labelColor=1a0a2e)
![License](https://img.shields.io/badge/license-MIT-C084FC?style=flat-square&labelColor=1a0a2e)
![Dark Mode](https://img.shields.io/badge/dark%20mode-required-4c1d95?style=flat-square&labelColor=1a0a2e)

<br/>

</div>

---

## // Overview

Amethyst replaces YouTube's default dark theme with a cohesive deep purple palette — from near-black `#0d0618` backgrounds to vibrant `#A855F7` accents — using glassmorphism-style surfaces, blur backdrops, and purple-tinted borders throughout the entire interface.

Every section is covered: masthead, sidebar, player, watch page, comments, feed, menus, channel pages, live chat, and miniplayer.

---

## ◈ Color Palette

| Role | Hex | Usage |
|------|-----|-------|
| Base background | `#0d0618` | Page bg, deepest surfaces |
| Surface | `#2d1060` @ 50% | Panels, drawers, dropdowns |
| Mid tone | `#4c1d95` @ 40% | Cards, chips, inputs |
| Primary accent | `#7C3AED` | Buttons, borders, highlights |
| Hover accent | `#A855F7` | Hover states, active elements |
| Highlight | `#C084FC` | Text accents, icon tints |
| Light text | `#ede9fe` | Text on colored surfaces |

---

## ▸ What's Covered

<details>
<summary><b>UI & Navigation</b></summary>

- Frosted glass masthead with purple border
- Auto-hide sidebar with blur backdrop
- Search bar with purple focus ring
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

- Description card with purple border
- Action buttons (like, share, save) purple-tinted
- Chapter markers with purple timestamps
- Gaming info card
- Merch shelf and rich header cards

</details>

<details>
<summary><b>Comments</b></summary>

- Author name pill chip (purple background)
- Submit button uses primary accent color
- Emoji picker with glass surface
- Creator heart in purple

</details>

<details>
<summary><b>Feed & Thumbnails</b></summary>

- Rounded thumbnails (12px)
- Duration badge with dark purple + blur
- Feed filter chips with purple tint
- Post cards with subtle purple surface
- Show more button styled

</details>

<details>
<summary><b>Menus, Popups & Dialogs</b></summary>

- All dropdowns: glass surface + purple border
- Notification center
- Account menu
- Save to playlist dialog
- Share panel
- Context menus

</details>

<details>
<summary><b>Channel Page</b></summary>

- Header backdrop blur with purple tint
- Tab bar with glass surface
- Avatar rounded corners throughout

</details>

<details>
<summary><b>Live Chat & Miniplayer</b></summary>

- Chat header with purple tint
- Input area transparent
- Miniplayer with purple border + blur

</details>

---

## ↓ Installation

**1. Install the extension**

| Browser | Link |
|---------|------|
| Chrome | [Chrome Web Store](https://chrome.google.com/webstore/detail/enhancer-for-youtube/ponfpcnoihfmfllpaingbgckeeldkhle) |
| Firefox | [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/enhancer-for-youtube/) |
| Edge | [Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/enhancer-for-youtube/dlgfaleeejmphhnemjgiaekdbonkagkd) |

**2. Copy the CSS**

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/amethyst-youtube.git

# Or just grab the file directly
curl -O https://raw.githubusercontent.com/YOUR_USERNAME/amethyst-youtube/main/enhancer-youtube-purple.css
```

**3. Paste into Enhancer**

```
Enhancer for YouTube → [ Settings ] → Custom CSS → paste → Save
```

**4. Reload YouTube** — done.

---

## § Requirements

- **Enhancer for YouTube** `3.0.17` or later
- YouTube **dark mode** enabled (Settings → Appearance → Dark theme)
- Browser hardware acceleration **on** (for `backdrop-filter` blur effects)
- Tested on **Chrome 120+** / **Firefox 121+**

---

## ! Notes

> **Sidebar auto-hide** — this CSS handles visuals only. The hide/show behavior requires the JavaScript snippet to be enabled inside Enhancer for YouTube's settings separately.

> **backdrop-filter support** — all blur effects use CSS `backdrop-filter`. If panels appear solid instead of frosted, check that GPU acceleration is enabled in `chrome://settings` → System.

> **YouTube UI updates** — YouTube frequently changes its internal class names. If something breaks after a YouTube update, open an issue and I'll push a fix.

---

## ~ Customization

All colors are defined as CSS variables at the top of the file. To change the accent color, edit the `:root` block:

```css
:root {
  --yt-purple-primary: #7C3AED;  /* change this */
  --yt-purple-accent:  #A855F7;  /* and this */
  --yt-purple-hi:      #C084FC;  /* highlight */
}
```

---

## * License

MIT — do whatever you want, credit appreciated but not required.

---

<div align="center">

made with ♥ 

</div>
