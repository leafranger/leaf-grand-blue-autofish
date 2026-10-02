# Getting started

From download to your first fishing session. It takes about ten minutes, most of it the calibration.

## 1. Install

1. Download `Leafs-Grand-Blue-Autofish-v0.1.1.zip` from the [latest release](../../../releases/latest). If you want to check it first, see [Verify your download](VERIFY.md).
2. Unzip the **whole folder** to a place you can write to, such as `Documents`. Do not run it from inside the zip, do not move the `.exe` out of its folder, and avoid `C:\Program Files`. The app saves its settings, calibration and sessions next to itself.
3. Double-click **Leaf's Grand Blue Autofish.exe**.

If Windows shows "Windows protected your PC", choose **More info** and then **Run anyway**. The app is not code-signed; [the FAQ explains why](FAQ.md#why-does-windows-or-my-antivirus-complain).

## 2. First start

- A short welcome page, then the **licence**, **privacy notice** and **third-party notices** are shown one at a time. Scroll each one to the end, tick the box, and press Next. You can read them again later from the heart tab.
- If your PC lacks Microsoft's Visual C++ runtime, a screen explains it and offers to download it from Microsoft or to open Microsoft's page so you can do it yourself. Nothing is downloaded unless you click.
- The app then opens, and because nothing is calibrated yet, the **calibration** opens by itself.

## 3. Calibrate

Open Roblox, join Grand Blue, stand where you fish, and click **Start calibration**. Each step explains what to do with a picture, you do it and press Continue, and the app checks its own work before moving on. A miss tells you what was wrong and offers Retry. Nothing is saved unless every step passes.

| Step | You | The app |
|---|---|---|
| 1. Roblox | Have the game open and stand where you fish | Finds the Roblox window and loads the text reader |
| 2. Cast position | Click the open water where it should cast | Remembers the spot |
| 3. Rod hotbar key | Press the key that takes out your rod | Shows it back so you can confirm |
| 4. Chat button | Open the chat, drag a box around its button | Checks it reads as lit, then closes the chat |
| 5. Menu button | Open the menu, drag a box around the whole button | Reads it, then closes the menu |
| 6. Backpack button | Open the backpack, drag a box around the whole button | Reads it, then closes the backpack |
| 7. Leaderboard | Open it and click its close button | Checks it is open, then closes it |
| 8. Bait panel | Equip your rod and drag a box around the BAIT panel | Uses it to tell whether the rod is equipped |
| 9. Checks | Hands off | Opens and closes the menu and backpack, and re-equips the rod, three times each |
| 10. SHAKE button | Hands off (do not click SHAKE yourself) | Casts, finds the SHAKE button, learns its size, and clicks until a fish bites |
| 11. Reeling bar | Drag a box around the long bar with the fish on it | Reads it from a picture saved at the bite |
| 12. Test catches | Let it run for a few minutes | Catches three fish and checks the reeling, the rarity badge and the catch message |
| 13. Done | | Saves everything as a calibration profile |

Boxes can be adjusted after you draw them: drag a corner to resize, or the middle to move. A magnified preview sits next to the box. If boxes land in the wrong place (several monitors, remote desktop), turn on **Draw on a separate screenshot window** at the bottom of the calibration window.

**If the SHAKE button is not found (step 10) or the reeling bar is not in the saved pictures (step 11)**, the miss notice shows a second button, **Draw it myself**. It casts again, takes a picture at the right moment, and lets you draw the box yourself.

## 4. Fish

Click **Start fishing**, or press **F8** in the game. The dashboard shows casts, catches, session time and profit, and a table of every catch. Press **F8** again to stop and **F10** to pause. See [Hotkeys](HOTKEYS.md) for the rest.

While fishing, keep Roblox in front. The app pauses by itself when you switch to another window and carries on when you come back.

## 5. After a session

- **Inventory** keeps every session: charts of rarity and accuracy, a searchable log, and CSV export.
- **Settings** has hotkeys, the rarities to let go, timings, the look of the app and sounds.
- **Calibration** shows your profiles. If something drifts, run the calibration again (F4 saves it as a new profile) or use a quick fix for a single piece.

Something not working? See [Troubleshooting](TROUBLESHOOTING.md).
