# Personal build of dwm

This is a personal fork of [Luke Smith's dwm](https://github.com/LukeSmithxyz/dwm) (upstream `v6.5`), maintained on the `personal-patches` branch.

## Branching

Active development happens on `personal-patches`. The `master` branch tracks upstream so the patch set can be rebased cleanly onto new upstream releases.

```bash
git checkout personal-patches
make clean && make
sudo make install
```

## Patches and features

- [autostart](https://dwm.suckless.org/patches/autostart/): runs `~/.local/share/dwm/autostart.sh` once at startup.
- [alwayscenter](https://dwm.suckless.org/patches/alwayscenter/): new floating windows are centered on the current monitor's window area.
- [movestack](https://dwm.suckless.org/patches/movestack/) / stacker: move the selected client up/down the stack with <kbd>super+shift+j/k</kbd>.
- [cyclelayouts](https://dwm.suckless.org/patches/cyclelayouts/): cycle through layouts forward/backward with <kbd>super+shift+period</kbd> / <kbd>super+shift+comma</kbd>.
- [hide vacant tags](https://dwm.suckless.org/patches/hide_vacant_tags/): only tags with clients or the selected tag are drawn in the bar.
- [barpadding](https://dwm.suckless.org/patches/barpadding/): configurable vertical/horizontal padding around the bar (`vertpad` / `sidepad` in `config.h`).
- [urgentborder](https://dwm.suckless.org/patches/urgentborder/): urgent clients use a distinct border color.
- [warp](https://dwm.suckless.org/patches/warp/): cursor warps to the center of the focused window on keyboard-driven focus changes.
- [swallow](https://dwm.suckless.org/patches/swallow/): terminal-run programs temporarily take the terminal's place.
- [scratchpad](https://dwm.suckless.org/patches/scratchpad/): dropdown terminals/calculator via <kbd>super+shift+return</kbd> and <kbd>super+'</kbd>.
- [vanitygaps](https://dwm.suckless.org/patches/vanitygaps/): gaps across all layouts.
- [sticky](https://dwm.suckless.org/patches/sticky/): make windows sticky with <kbd>super+s</kbd>.
- [shiftview](https://dwm.suckless.org/patches/nextprev/): cycle through tags with <kbd>super+g</kbd> / <kbd>super+;</kbd>.
- [xresources](https://dwm.suckless.org/patches/xresources/): colors and variables loaded from Xresources.
- True fullscreen (<kbd>super+f</kbd>) with focus locking.
- Extra layouts: bstack, fibonacci, deck, centered master, centered floating master, floating.

## Aesthetic tweaks

- Nord-inspired dark color palette.
- Primary font: `JetBrainsMono Nerd Font:size=11`, with monospace and NotoColorEmoji fallbacks.
- Modern gap/border sizing: `borderpx 2`, tuned `gappih/gappiv/gappoh/gappov`.

## FAQ

> What are the bindings?

This is suckless; the source is the documentation. See [`config.h`](config.h) for all keybindings. Luke's system overview is still available in `larbs.mom` and via <kbd>super+F1</kbd>.
