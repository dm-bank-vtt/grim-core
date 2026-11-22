# Grim Core

Foundry VTT V13–V14 · © DM Bank

Discord: https://discord.gg/XWfgWKpxJp

---

One settings panel for every Grim module. Pick a colour theme here and every active Grim module changes with it, for the GM and every player.

## How to use

1. Open **Game Settings → Configure Settings → Grim Core → Open Grim Core** (GM only).
2. Pick a theme and press **Apply to all**.

| Module | What follows |
| --- | --- |
| Grim Almanac, Grim Theater of Mind, Grim Pulse, Grim Jukebox, Grim Stage Pacer, Grim Target | Full theme |
| Grim FateRoll | Sigil (accent) colour |
| Grim VN Stage | GM panel colours |
| Grim Encounter | Launcher panel and the initiative screen (cards, buttons) |

## Themes

- **Crimson, Ash, Amethyst, Abyss** — the four built-in Grim themes (Abyss is the theme Almanac and Theater call Sapphire).
- **Custom** — any accent colour, on dark or light surfaces, with a slider for how much of the accent shows in backgrounds. Colours that carry a meaning (friendly / hostile, signal lamps, Natural 20 gold) are left alone.

Untick a module under **Modules that follow** to leave it on its own colours. **Back to Crimson** restores the default theme.

Grim Core works with any number of Grim modules installed; the ones that are not active are listed as Not active.

## Macro API

```js
const core = game.modules.get("grim-core").api;
core.open();
core.setTheme({ preset: "abyss" });
core.setTheme({ preset: "custom", accent: "#2fa37a", base: "dark", tint: 100 });
core.palette(); // current colours, e.g. { blood: "#18956d", bone: "#d7e5df", ... }
```

## Install

In Foundry, go to **Add-on Modules → Install Module**, paste this link into **Manifest URL** and press **Install**:

```
https://github.com/dm-bank-vtt/grim-core/releases/latest/download/module.json
```

Then enable Grim Core under Manage Modules in your world. Foundry offers each new version as an update.

Players install nothing; only the machine hosting the game needs the module. On The Forge, install it with the same manifest link.

**Installed an earlier copy?** Install again from the link above so Foundry can update it. Your world's settings are kept.

## Support & Updates

Join the DM Bank Discord for updates and support: https://discord.gg/XWfgWKpxJp

## Terms of Use

- Free to download and use.
- Do not sell this module or its files.
- © DM Bank. All rights reserved.
