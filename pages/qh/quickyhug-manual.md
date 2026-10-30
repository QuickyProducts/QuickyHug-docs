---
title: QuickyHug HUD Manual
sidebar: home_sidebar
permalink: quickyhug-manual.html
keywords: quickyhug, hug hud, couple, manual, help, partner, pose
toc: true
---

QuickyHug is a hug HUD for two. You wear it, pick a pose and a partner nearby, and both of you are animated together. Your avatar follows your partner, so you can hug anywhere without furniture. The arrows of the HUD fine-tune your position; the HUD remembers it for every partner and pose.

{% include note.html content="Draft. Screens and numbers follow HUD version 1.1." %}

## Wearing the HUD

1. Find **QuickyHug HUD** in your inventory and choose **Add** (or **Wear**). It attaches as a HUD.
2. A new HUD starts switched off: you only see one round button with the hug symbol (two figures with a heart).
3. Click it to switch the HUD on. The button row appears.

For the best result, read [Recommended viewer settings](quickyhug-viewer-settings.html) once. It explains RLV and one debug setting that makes small turns visible right away.

## Starting a hug

1. Click **Poses** in the button row (13 in the picture below) and choose a pose.
2. If your last partner is still near you, the hug starts with them. Otherwise a list of people within 20 m opens: choose your partner.
3. Your partner gets a permission request to be animated. Once they accept, the hug starts and the full HUD opens.

Your partner does not need a HUD. If they don't answer the request, they get a short reminder after 20 seconds.

{% include tip.html content="When the hug starts, your partner gets a chat hint: they can type <code>/11 pose</code> to choose a pose themselves and <code>/11 stop</code> to end the hug." %}

## The button row

The button row is always visible while the HUD is switched on, with or without a hug.

<figure class="hud-map" style="max-width:600px;margin:1.5rem auto">
<svg width="100%" viewBox="0 0 600 190" role="img" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<title>QuickyHug button row</title>
<desc>The four buttons of the QuickyHug button row with numbered callouts.</desc>
<image href="images/QuickyHug-block.png" xlink:href="images/QuickyHug-block.png" x="44" y="50" width="512" height="128"/>
<g stroke="#5b6b7e" stroke-width="1.2">
<line x1="108" y1="32" x2="108" y2="54"/>
<line x1="236" y1="32" x2="236" y2="54"/>
<line x1="364" y1="32" x2="364" y2="54"/>
<line x1="492" y1="32" x2="492" y2="54"/>
</g>
<g font-family="Arial,Helvetica,sans-serif" font-size="13" text-anchor="middle">
<circle cx="108" cy="20" r="12" fill="#1f80c0"/><text x="108" y="20" fill="#fff" dominant-baseline="central">12</text>
<circle cx="236" cy="20" r="12" fill="#1f80c0"/><text x="236" y="20" fill="#fff" dominant-baseline="central">13</text>
<circle cx="364" cy="20" r="12" fill="#1f80c0"/><text x="364" y="20" fill="#fff" dominant-baseline="central">14</text>
<circle cx="492" cy="20" r="12" fill="#1f80c0"/><text x="492" y="20" fill="#fff" dominant-baseline="central">15</text>
</g>
</svg>
<figcaption>Button row</figcaption>
</figure>

12. **Turn left**: turns you 10° to the left. Works with and without a hug.
13. **Poses**: opens the pose menu. Without a hug, choosing a pose starts one (see above).
14. **Turn right**: turns you 10° to the right.
15. **Power**: switches the HUD off. A running hug ends, and only one round button with the hug symbol stays. Click it to switch the HUD on again.
{: start="12"}

## The HUD during a hug

While you hug, the control cross opens below the button row. The numbers match the list that follows.

<figure class="hud-map" style="max-width:640px;margin:1.5rem auto">
<svg width="100%" viewBox="0 0 760 430" role="img" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
<title>QuickyHug HUD control map</title>
<desc>The HUD during a hug with numbered callouts pointing to each control.</desc>
<defs><marker id="qharrow" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse"><path d="M2 1L8 5L2 9" fill="none" stroke="context-stroke" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></marker></defs>
<image href="images/QuickyHug-HUD.png" xlink:href="images/QuickyHug-HUD.png" x="118" y="24" width="500" height="386"/>
<g stroke="#5b6b7e" stroke-width="1.2" fill="none">
<line x1="52" y1="81" x2="150" y2="81" marker-end="url(#qharrow)"/>
<line x1="52" y1="211" x2="150" y2="211" marker-end="url(#qharrow)"/>
<line x1="52" y1="349" x2="150" y2="349" marker-end="url(#qharrow)"/>
<line x1="262" y1="406" x2="322" y2="312" marker-end="url(#qharrow)"/>
<line x1="262" y1="48" x2="322" y2="114" marker-end="url(#qharrow)"/>
<line x1="466" y1="16" x2="512" y2="40" marker-end="url(#qharrow)"/>
<line x1="630" y1="16" x2="592" y2="40" marker-end="url(#qharrow)"/>
<line x1="703" y1="132" x2="528" y2="132" marker-end="url(#qharrow)"/>
<line x1="703" y1="214" x2="590" y2="214" marker-end="url(#qharrow)"/>
<line x1="703" y1="302" x2="528" y2="302" marker-end="url(#qharrow)"/>
</g>
<g font-family="Arial,Helvetica,sans-serif" font-size="13" text-anchor="middle">
<circle cx="422" cy="217" r="11" fill="#1f80c0"/><text x="422" y="217" fill="#fff" dominant-baseline="central">1</text>
<circle cx="40" cy="81" r="12" fill="#1f80c0"/><text x="40" y="81" fill="#fff" dominant-baseline="central">3</text>
<circle cx="40" cy="211" r="12" fill="#1f80c0"/><text x="40" y="211" fill="#fff" dominant-baseline="central">6</text>
<circle cx="40" cy="349" r="12" fill="#1f80c0"/><text x="40" y="349" fill="#fff" dominant-baseline="central">4</text>
<circle cx="250" cy="415" r="12" fill="#1f80c0"/><text x="250" y="415" fill="#fff" dominant-baseline="central">2</text>
<circle cx="250" cy="40" r="12" fill="#1f80c0"/><text x="250" y="40" fill="#fff" dominant-baseline="central">8</text>
<circle cx="455" cy="12" r="12" fill="#1f80c0"/><text x="455" y="12" fill="#fff" dominant-baseline="central">10</text>
<circle cx="642" cy="12" r="12" fill="#1f80c0"/><text x="642" y="12" fill="#fff" dominant-baseline="central">11</text>
<circle cx="715" cy="132" r="12" fill="#1f80c0"/><text x="715" y="132" fill="#fff" dominant-baseline="central">7</text>
<circle cx="715" cy="214" r="12" fill="#1f80c0"/><text x="715" y="214" fill="#fff" dominant-baseline="central">5</text>
<circle cx="715" cy="302" r="12" fill="#1f80c0"/><text x="715" y="302" fill="#fff" dominant-baseline="central">9</text>
</g>
</svg>
<figcaption>QuickyHug HUD during a hug</figcaption>
</figure>

1. **Poses**: opens the pose menu to change the pose (same as 13). The menu opens on the page of the current pose.
2. **Partner**: **End Hug** ends the hug, **New Partner** picks someone else nearby with the same pose, **Stop Partner** stops only your partner's animation.
3. **Resync**: restarts both animations at the same moment. Use it when the two of you drift apart, which happens over time on looped animations.
4. **Swap**: you and your partner trade animations.
5. **Move**: moves you forward, back, left and right, as seen from your camera. The three arrows per direction move 1 cm, 5 cm and 10 cm (the outer arrow moves furthest).
6. **Up / down**: raises or lowers you in the same three steps.
7. **End hug**: ends the hug. The HUD stays switched on.
8. **Info**: lists the HUD's scripts and versions in chat. Useful when you ask for support.
9. **Settings**: see [Settings dialog](#settings-dialog).
10. **Size + / −**: makes the whole HUD bigger or smaller on your screen.
11. **Minimize**: folds the HUD to a small round button with the hug symbol. The hug keeps running; click the button to open the HUD again.

<figure style="max-width:120px;margin:1rem auto;text-align:center">
<img src="images/QuickyHug-minimized.png" alt="Minimized HUD" width="96" height="96"/>
<figcaption>Minimized</figcaption>
</figure>

## Adjusting your position

Every move with the arrows (5, 6) and every turn (12, 14) is saved automatically, a moment after your last click:

- **For this partner and this pose.** Next time you hug the same person with the same pose, you are right back in place.
- **As your own start position** for this pose. With a partner you haven't hugged in this pose before, the HUD starts from your last adjustment.

**Settings > Reset Pos** forgets both and goes back to the creator's default for this pose.

{% include note.html content="Positions are stored for your role in the pose. When you swap (4), the HUD works out the matching position for the other side." %}

## Settings dialog

| Button | What it does |
|---|---|
| RESYNC | same as 3 |
| Reset Pos | back to the default position for this pose (see above) |
| Switch Lead | your partner leads and you follow them, or back (see below) |
| SWAP | same as 4 |
| Add Pose / Delete Pose / Rename Pose | manage poses, see [Poses and menus](quickyhug-poses.html) |
| Version | same as 8 |

Without a hug the dialog only shows the pose buttons and Version.

## Switch Lead: let your partner walk

Normally you follow your partner: they can walk, and you stay in your pose with them. **Switch Lead** turns this around: you walk freely and your partner follows you.

1. Your partner wears the **QuickyHug partner attachment**. You can give it to them; it is copy and transfer.
2. During a hug, choose **Settings > Switch Lead**. Your partner gets a dialog and agrees.
3. To switch back, choose **Switch Lead** again, or your partner clicks their attachment.

## Your partner's commands

Your partner types in local chat:

| Command | What it does |
|---|---|
| `/11 pose` | opens the pose menu for them |
| `/11 stop` | ends the hug |

Only your current partner can use them; anyone else saying them is ignored.

## Sitting

When you start a hug while sitting, the HUD only plays the animations: no following, no turning. Stand up first for the full function.

## Troubleshooting

| What you see | What to do |
|---|---|
| Your partner is not animated | They have to accept the permission request. Choose **New Partner** and the same person again to ask once more. |
| Small turns only show after several clicks | Set the debug setting from [Recommended viewer settings](quickyhug-viewer-settings.html). |
| You are pushed away from your partner | Move up a few centimetres (6). Very tall avatars can still bump into each other. |
| The animations drift apart | Click Resync (3). |
| Anything else | Click Info (8) and send the chat lines with your question. |
