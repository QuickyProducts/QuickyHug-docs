---
title: Recommended Viewer Settings
sidebar: home_sidebar
permalink: quickyhug-viewer-settings.html
keywords: quickyhug, rlv, rlva, debug settings, AvatarRotateThresholdSlow, hover, firestorm
toc: true
---

QuickyHug works in every viewer. Two settings make it look better. Both are set once in your own viewer and stay set.

| Setting | Why | Who |
|---|---|---|
| [RLV on](#rlv) | the animations keep their full hip movement | the person wearing the HUD |
| [AvatarRotateThresholdSlow = 5](#small-turns) | small turns show right away instead of after several clicks | everyone who wants to see the exact turn |

## RLV

### What the HUD does with RLV

To hug without bumping into each other, the HUD lifts you about 2 m above your partner and lowers your visible body by the same amount. How it lowers you depends on RLV:

- **With RLV** the HUD sets your viewer's hover height. The animations play untouched, including hip movements.
- **Without RLV** the HUD plays a lowering animation. It works everywhere, but it can stiffen the hips of some animations.

With RLV the HUD also turns you through RLV. It only uses these two commands: hover height and turning. It does not lock, restrict or detach anything, and it sets the hover height back to 0 when the hug ends.

{% include note.html content="If you use a hover height of your own, it is 0 after a hug. RLV cannot read your previous value, so set it again if you need it." %}

<!-- TODO: Absenkung 2,3 m ist im Test (follow 1.16). Hier "about 2 m" lassen oder anpassen, wenn entschieden. -->

### Turning RLV on

**Firestorm**

1. Open **Preferences** (Ctrl + P).
2. Go to **Firestorm > Extras**.
3. Tick **Allow Remote Scripted Viewer Controls (RLVa)**.
4. Restart the viewer. RLV only starts after a restart.

**Other viewers with RLVa** (for example Alchemy, Black Dragon, Catznip): look for **RLVa** in the preferences or in the **Advanced** menu, enable it and restart.

The official **Second Life Viewer** has no RLV. QuickyHug still works there, with the lowering animation.

To check: click **Info** on the HUD during a hug. The line of `[QH]follow` says `lowering: RLV hover` when RLV is used.

## Small turns

The turn buttons turn you 10° per click. Many viewers only turn the visible body once the difference is bigger than 60°, so you see the turn after the third click or later. The debug setting `AvatarRotateThresholdSlow` changes that.

1. Press **Ctrl + Alt + Shift + S** to open Debug Settings.
   - Firestorm: also **Advanced > Show Debug Settings**.
   - Second Life Viewer and Alchemy: if the shortcut doesn't work, press **Ctrl + Alt + D** first to show the **Advanced** menu, then choose **Advanced > Show Debug Settings**.
2. Type **Rotate** into the search field.
3. If **AvatarRotateThresholdSlow** shows up, change the value from **60** to **5**.
4. Close the window. The setting is kept.

If the setting doesn't show up, this viewer no longer has it (it was removed from viewers based on the Linden Lab code in 2024, for example Alchemy). Linden Lab fixed it again in Second Life Viewer 26.1, so updating or switching viewers may help.

This only changes what your own viewer shows. Everyone who wants to see the exact turn has to set it in their viewer. If 5 still feels slow, 1 works too; at 0 the body may twitch on the smallest movement.
