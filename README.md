# 💜 Nova UI (no longer being updated)

A styling enhancement for the Zen browser theme. Nova improves the visual consistency of the Zen theme by adjusting spacing, padding, borders, and overall layout

> **Fork note (v2.4):** this is a maintained fork of [qumeqa/nova](https://github.com/qumeqa/nova), which is archived. It was checked against Zen 1.23 and 1.24.
>
> **Find bar (v2.4):** Ctrl+F seemed to do nothing. The find bar did open, but 20px below the bottom of the page, out of sight.
>
> **Why:** newer Firefox lays out the page area as a CSS grid, with the find bar in its own row at the bottom. Nova positions the find bar `absolute` with `top: 20px`, and an absolutely positioned grid item is measured from its own grid row. That row starts at the bottom edge of the page, so the bar landed below it. Nova now places the find bar in the page's `browserstack` grid area, so it floats at the top as intended.
>
> **Tab shadow (v2.3):** the "Remove shadow from tabs" option no longer removed the selected tab's shadow.
>
> **Why:** Firefox renamed the variable Nova cleared, `--tab-selected-shadow`, to `--tab-box-shadow-selected`. Zen also now sets it on each `zen-workspace`, below the `#tabbrowser-tabs` element that Nova targeted. The option now clears the new variable on both elements, and still clears the old one for older Zen builds.
>
> **Also:** removed a leftover `@import` of `modules/tabs.css`, a file merged into `other.css` long ago, which only caused a failed load. Every other selector, setting and Zen variable Nova uses was checked and still works.
>
> Install in Sine from `https://github.com/LoopRook/nova`. If you have the original installed, remove it first.

![Nova UI Theme](https://raw.githubusercontent.com/LoopRook/nova/refs/heads/main/img/main.jpg)

> [!NOTE]
> Screenshot with "New Icons" mod

## ✨ About

Nova UI is a mod that refines the Zesn theme. It standardizes spacing, adjusts padding for UI elements, and improves the visual consistency of popups, tabs, menus, and panels. The mod maintains the Zen theme's original functionality while providing a more unified visual presentation

![Settings](https://raw.githubusercontent.com/LoopRook/nova/refs/heads/main/img/other.jpg)

## 🔮 What It Changes

- **Spacing & Padding** — Standardized padding values across buttons, menu items, and panels
- **Popup Styling** — Refined styling for menus, subviews, and dropdown elements
- **Border & Corner Radius** — Consistent border radius for popups and panels
- **Essentials Tabs** — Simplifies background colors, making them like regular tabs
- **Scrollbar Appearance** — Improved scrollbar styling

## ⚙️ Configuration

- **Enable Border** — Add visible borders around all popups and panels
- **Bleeding Corners Fix integration** — Fix white outlines on rounded corners
- **New Essentials background colors** — Simplified background like regular tabs
- **Quietify Integration** — Add a calm visualizer type of animation to mute button to use with style and ease
- **Custom Font** — Replaces the interface font with any font you want

![Settings](https://raw.githubusercontent.com/LoopRook/nova/refs/heads/main/img/settings.png)

## 🎯 Recommended Mods

For the best experience, use Nova UI together with:

- **"New Icons"** — Modern icon set that perfectly complements Nova ([fixed fork for Zen 1.23+](https://github.com/LoopRook/zen-icons))
- **"Floating Findbar"** — Floating find-in-page search bar

## 🚀 Future Plans

- **Website Information** — Improved website information popup styling
- **Firefox style buttons** — Add tab style with left and right margin and rounded corners

## ✅ Installing

> [!IMPORTANT]
> Before installing Nova UI, you must first install [Sine](https://github.com/CosmoCreeper/Sine), a mod/theme manager for Firefox-based browsers

### Install Nova UI

Once Sine is installed, you can install Nova UI through the Sine marketplace
