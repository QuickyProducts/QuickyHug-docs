---
title: Poses and Menus
sidebar: home_sidebar
permalink: quickyhug-poses.html
keywords: quickyhug, poses, add pose, hug box, menu, submenu, notecard, QH-Menu
toc: true
---

A pose in QuickyHug is a pair of animations: one for each of you. This page shows how to add your own poses, sort them into menus and manage them.

## The pose menu

Click **Poses** on the HUD. The menu works like a sitter menu:

- Buttons with a star, like `Standing*`, open a submenu.
- `New*` holds poses that are not sorted into a menu yet. It only appears while it has poses.
- **[BACK]** goes one menu up, **[CANCEL]** closes the menu, `<<<` and `>>>` turn the page.
- **[POSES]** opens the edit dialog for the menu you are in (owner only).

The menu opens where your current pose is.

## Adding a pose with the QuickyHugBox

The easiest way. The box finds out which animation is whose and adds the pose for you.

1. Click **Settings > Add Pose > Hug Box**. The box appears in front of you. You need rez rights on the land.
2. Drag the two animations from your inventory onto the box (hold **Ctrl** while dragging).
3. Touch the box. It sends both animations to your HUD, the pose is added, and the box disappears with a few hearts.

<figure class="hud-map" style="max-width:560px;margin:1.5rem auto">
<svg width="100%" viewBox="0 0 640 330" role="img" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<title>QuickyHugBox</title>
<desc>The QuickyHugBox waiting for animations (left) and ready (right), with numbered callouts.</desc>
<defs><marker id="qbarrow" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse"><path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></marker></defs>
<image href="images/QuickyHugBox.png" xlink:href="images/QuickyHugBox.png" x="64" y="30" width="512" height="256"/>
<g stroke="#5b6b7e" stroke-width="1.2" fill="none">
<line x1="192" y1="306" x2="192" y2="262" marker-end="url(#qbarrow)"/>
<line x1="448" y1="306" x2="448" y2="262" marker-end="url(#qbarrow)"/>
</g>
<g font-family="Arial,Helvetica,sans-serif" font-size="13" text-anchor="middle">
<circle cx="226" cy="84" r="12" fill="#1f80c0"/><text x="226" y="84" fill="#fff" dominant-baseline="central">1</text>
<circle cx="192" cy="316" r="12" fill="#1f80c0"/><text x="192" y="316" fill="#fff" dominant-baseline="central">2</text>
<circle cx="448" cy="316" r="12" fill="#1f80c0"/><text x="448" y="316" fill="#fff" dominant-baseline="central">3</text>
</g>
</svg>
<figcaption>QuickyHugBox</figcaption>
</figure>

1. **Drop here**: the arrow shows where the animations go. Drag them onto any side of the box.
2. **Waiting**: the box is matt while it is empty. With one animation, two sides light up. The floating text counts the animations (`1/2`) and the minutes until the box cleans itself up.
3. **Ready**: with two animations the whole box glows. Touch it.

**Which animation is whose:** the box sorts the two animations by their names (`male` / `female` anywhere in the name, or an ending `-m` / `-f`). If the names don't tell, it asks which animation is your hug partner's. In the hug you play yours and your partner the other one; **Swap** trades them any time.

**Good to know**

- Without a menu notecard the box takes exactly two animations. Anything else you drop in comes back to you.
- Animations need copy permission. Second Life does not let a worn HUD take no-copy animations.
- A worn HUD that you can transfer does not take no-transfer animations either. The box tells you; then rez your HUD on the ground and drag the animations into its contents.
- **Pose names from the file name:** an animation named `Standing@Name@...` or `Floor@Name@...` gets the pose name `Name` (at most 24 characters). If that name is already taken, a number is added. Everything else keeps its file name until you rename it.
- Without use, the box deletes itself after 10 minutes and gives back what can't be copied.

### Many poses at once: menu notecard

Put a notecard named **`QH-Menu`** into the box together with any number of animations. Touching the box sends all animations the HUD is missing and then the notecard, which builds the menus. The format is described [below](#menu-notecard-qh-menu).

## Adding a pose by hand

1. Drag the two animations into the HUD's contents (rez the HUD on the ground, **Edit > Contents**).
2. Named `<name>-male` and `<name>-female`, they become a pose by themselves.
3. Any other names: **Settings > Add Pose > Pair Anims** asks for your animation, your hug partner's animation and a name.

New poses land in `New*` and are reported in chat.

## Editing poses and menus

Open the menu you want to change and click **[POSES]**.

| Button | What it does |
|---|---|
| Add Pose | how to add poses, with **Hug Box** and **Pair Anims** |
| Delete Pose | removes a pose and its animations (if no other pose uses them). Paired poses can also be **Unpaired**: the animations stay. |
| Rename Pose | the name on the button, at most 24 characters. Empty goes back to the file name. |
| Move Pose | choose a pose, open the target menu and press **[HERE]**. Target `New*` takes it out of all menus. Afterwards the menu you came from opens again, so you can sort many poses in a row. |
| New Menu | a submenu inside the menu you are in |
| Rename Menu / Delete Menu | the menu you are in, so they only appear inside a submenu: open the submenu, then **[POSES]**. Deleting moves its poses and submenus one level up. |
| Load Card | reads the `QH-Menu` notecard in the HUD |
| Help | the help dialog: manual, support and versions, see [Help](quickyhug-manual.html#help) |

## Menu notecard `QH-Menu`

A notecard named `QH-Menu` in the HUD's contents builds menus and sorts poses. The HUD reads it when it changes, or with **[POSES] > Load Card**. A summary in chat lists poses it could not find.

```
# lines starting with # are comments
!clear
[Standing]
hug1
kiss
[Standing/Romantic]
slowdance
Tango = Tango Lead A | Tango Follow B
[Lying]
cuddle
```

| Line | Meaning |
|---|---|
| `[path]` | a menu, submenus separated by `/`. Missing menus are created, existing ones are found by name. |
| `hug1` | a pose by its file name without `-male` / `-female` |
| `Name = me \| partner` | pairs two animations under a name, like Pair Anims: first your animation, then your hug partner's. **Swap** trades them during the hug. |
| `!clear` | removes all menus first, so all poses start in `New*`. Only useful as the first line. |

Without `!clear` the notecard adds to what is there: poses it names move to the end of their menu, everything else stays where it is. For an exact order, start with `!clear` and list every pose.
