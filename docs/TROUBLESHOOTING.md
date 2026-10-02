# Troubleshooting

Find your problem below. If none of it helps, ask on [Discord](https://discord.gg/AC8qRsUHsc), the quickest place to get an answer, or [open an issue](../../../issues/new/choose) and fill in the form (issues are read, but less often).

## The app does not open, or the window is blank

- **An error mentioning `Python.Runtime.Loader.Initialize` (or "Windows is blocking this program's files").** Windows marks files from a browser download as coming from the Internet, and a part of the app refuses to load marked files. Version 0.1.1 and later clear that mark by themselves. On 0.1.0, or if it still happens: right-click the **.zip you downloaded**, choose **Properties**, tick **Unblock** at the bottom, press OK, and unzip it again into a new folder. If you already unzipped it, open PowerShell and run `Get-ChildItem -Recurse "C:\path\to\the\folder" | Unblock-File` (with the real folder path), then start the app again.

- **Unzip the whole folder** and run the `.exe` from inside it. Running it from inside the zip, or moving the `.exe` somewhere else on its own, leaves out the files it needs (for example `python312.dll`).
- **Do not put it in `C:\Program Files`.** The app saves its files next to itself and needs a folder you can write to, such as Documents.
- **An antivirus may have removed or blocked a file.** Look in your antivirus's quarantine, restore the app's files, and add its folder as an exception, or re-download and unzip again.
- **A blank window** usually means Microsoft Edge WebView2 is missing or damaged. It comes with Windows 10 and 11; you can reinstall it from Microsoft.
- **A message about a Microsoft component** (the Visual C++ runtime) is explained on the first-start screen. Let the app download it, or install it from Microsoft's page and press "check again".
- If the app closes by itself, look for **`crash-log.txt`** next to the `.exe` and attach it to your issue. A short message also appears when it can.

## A calibration step will not pass

Each miss says what was wrong. The usual causes:

- **Chat, menu, backpack, leaderboard.** The panel has to be in the state the step shows (open or closed) when you press Continue and draw the box. Draw the box tight around the button, as in the picture.
- **Bait panel.** Equip your rod first so the BAIT panel is visible.
- **Boxes land in the wrong place** (several monitors, remote desktop, display scaling). Turn on **Draw on a separate screenshot window** at the bottom of the calibration window.
- **The text reader is not available.** The steps that read on-screen text are skipped and the app tells you; everything else still works.
- You can always press **Retry**, or **Cancel** and start again. Nothing is saved until every step passes.

## Step 10: the SHAKE button is not found

- Do not click the button yourself; the app clicks it.
- Make sure the rod is equipped and the cast spot is open water.
- Wait a minute between attempts if you retried straight away: a SHAKE from the previous cast may still be pending in the game, and the next cast can then do nothing.
- If it still misses, press **Draw it myself**. The app casts, takes a picture when the button is up, and you draw a box around it.

## Step 11: the reeling bar is not in the pictures

The pictures are taken when a fish bites, and the fish can be gone before they are. Press **Draw it myself**: the app casts again, clicks SHAKE until a fish bites, takes fresh pictures, and you draw the box on those. If SHAKE is not being clicked, click it yourself while it waits.

## SHAKE is not being clicked while fishing

- Turn on quick fixes (Calibration page) and use **F6** with the SHAKE button on screen to draw it by hand.
- Press **F3** while the SHAKE button is up and not being clicked. It saves a report, with a picture of the game window only, in the `shakereports` folder; attach it to an issue.
- Very dark scenes can make the button harder to confirm. Fishing somewhere brighter, or redrawing the button with F6, usually fixes it.

## The mouse button is stuck down

Click the left mouse button once, or press the pause hotkey (**F10**). The app lets go of the mouse every time it stops, pauses or hits an error, so a stuck button is a bug worth reporting.

## A hotkey does nothing

Another program is probably using that key. The activity log names the key it used instead. Rebind either one under **Settings → Hotkeys**. Quick-fix keys do nothing until you turn quick fixes on in the Calibration page.

## It pauses by itself

It pauses whenever the window in front is not Roblox: a browser tab or chat window with "Roblox" in its title does not count. Bring the game to the front and it carries on.

## "The workstation is locked"

Windows blocks mouse and keyboard input while the PC is locked. The app keeps waiting and carries on when you unlock it.

## Catches show as unread or unknown

Open the Calibration page, turn on quick fixes and use **F11** to box the area where the catch message appears. This is optional; the app normally finds it by itself.

## Start again from scratch

Close the app and delete `config.json`, `calibration_profiles.json` and the `assets\profiles` folder, then start it and calibrate again. Your sessions are kept in the `sessions` folder.

## What to put in a bug report

On [Discord](https://discord.gg/AC8qRsUHsc) or in the [issue form](../../../issues/new/choose), include the version, your Windows version, the game's resolution, what happened and `crash-log.txt` if there is one. A screenshot of the app window helps. Please do not post pictures that show other players' names or chat.
