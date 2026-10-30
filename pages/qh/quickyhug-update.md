---
title: Updating to a New HUD
sidebar: home_sidebar
permalink: quickyhug-update.html
keywords: quickyhug, update, transfer, new version, move poses
toc: true
---

When you get a new version of the QuickyHug HUD, your poses, menus and saved positions can move over from the old HUD. The old HUD sends them to the new one.

## How to

**Both HUDs on the ground (recommended)**

1. Rez the **new** HUD on the ground.
2. Rez the **old** HUD next to it, at most 10 m away.
3. After a few seconds the old HUD asks whether to transfer. The dialog shows both versions. Click **Transfer**.
4. Both HUDs report in chat when they are done. Take the new HUD and wear it; you can delete the old one.

**New HUD worn**

1. Wear the new HUD.
2. Rez the old HUD on the ground and click **Transfer** in its dialog.

This works too, but Second Life does not let a worn HUD that you can transfer take no-transfer animations. The old HUD lists them; transfer again with both HUDs on the ground to bring them over.

{% include tip.html content="The order matters: the HUD that was rezzed last asks. If the new HUD asks instead, it warns that the other HUD is not newer. Click Cancel and rez the old HUD again." %}

## What moves over

| | |
|---|---|
| Poses | all your poses, with their names and the animations the new HUD is missing |
| Menus | merged with the menus of the new HUD (see below) |
| Positions | your saved positions per partner and your own start positions |
| Last pose | the pose the menu opens with |

What stays as it is in the new HUD: the creator's default positions, the HUD size and the layout.

Animations without copy permission are **moved** from the old HUD to the new one, not copied.

## How menus are merged

- Menus with the same name become one menu.
- Menus and poses that only the new HUD has stay where they are.
- Your poses go back to the menu they were in in your old HUD, also if the new HUD sorted them differently.
- If the new HUD has a different pose with the same name as one of yours, your pose is added under a new name, in its old place, without its saved positions. The chat summary names these poses.

## If something goes wrong

- **No dialog appears:** the old HUD only looks for the new one right after it is rezzed. Take it and rez it again. Check that the new HUD is worn or lies within 10 m.
- **The transfer stops halfway:** just rez the old HUD again and transfer once more. Everything that already moved over is skipped.
- **"refused the transfer … newer HUD version":** you are moving data from a newer HUD into an older one. Transfer into a HUD of the same or a newer version.
- **Old HUD from before version 1.1:** it doesn't have the transfer script yet. Ask for the script `[QH] transfer`, drop it into the rezzed old HUD, and it starts at once.
