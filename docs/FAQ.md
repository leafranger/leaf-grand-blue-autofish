# FAQ

## Will I get banned?

It can happen. Automation, macros and bots can go against Roblox's Terms of Use and the rules of individual games, whether or not they are enforced, and Roblox or the game's developers can act on your account. The app does not try to hide itself from them. Using it is at your own risk; the [licence](../LICENSE.txt) says so too. If your account matters to you, do not use it.

## Does it read or change the game?

No. It does not touch the game's files or memory, and it does not talk to Roblox's servers. It takes pictures of your screen, reads them, and then moves the mouse and presses keys, like a person would.

## Is it safe to run?

It runs entirely on your PC with no accounts and no tracking, and it makes no network connections of its own (the one optional exception is downloading Microsoft's Visual C++ runtime if your PC lacks it, and only if you click to let it). The source code is not published, so you cannot read it, but you can [verify that the file you downloaded is the one that was released](VERIFY.md), and see what it saves in the [privacy notice](../legal/PRIVACY.txt).

## Why does Windows or my antivirus complain?

Two reasons:

- **The app is not code-signed.** A signing certificate costs money every year and this is a free project, so Windows shows "Windows protected your PC" and calls the publisher unknown.
- **It does things antivirus software watches for.** It listens for hotkeys and sends mouse clicks and key presses. Any program that does that can trigger a heuristic warning.

Check your download against the published SHA256 and the scan result in [Verify your download](VERIFY.md) before you run it. If your antivirus quarantines the app, you can restore it and add its folder as an exception, or decide not to use it.

## Where is my data? How do I uninstall?

Everything is saved in the app's own folder: your settings and calibration, your sessions, and your catch history. There is no installer and nothing in the registry. To remove the app, delete its folder. To keep your sessions when you move to a new version, copy the `sessions` folder across.

## Can I use my PC while it fishes?

Not really. It moves the mouse and clicks, and it pauses by itself when Roblox is not the window in front. Leave the game in front and let it run.

## Do I have to calibrate again?

When you change the Roblox window's size or position, switch monitors, or change your display scaling, run the calibration again (**F4**, saved as a new profile) so the boxes match your screen. Up to five profiles are kept, so you can switch between setups.

## Does it work on several monitors?

It is built to. If the boxes land in the wrong place during calibration (several monitors, remote desktop), turn on **Draw on a separate screenshot window** at the bottom of the calibration window.

## Which game is it for?

Grand Blue on Roblox. It reads Grand Blue's fishing interface, so it will not work in other games unless their minigame happens to look the same.

## How do I update?

There is no automatic update check, because the app does not go online. New versions are published on the [Releases page](../../../releases). Download the new zip and unzip it as a new folder. Your calibration lives in the old folder, so run the calibration again, or copy `config.json`, `calibration_profiles.json` and the `assets\profiles` folder across.

## Is the source code available?

No. The app is free to use, but its source is not published. See the [licence](../LICENSE.txt).

## Does it cost anything?

No. If it saved you time, a tip is welcome and never expected: [Ko-fi](https://ko-fi.com/leafranger).

## I found a bug or I need help

First try [Troubleshooting](TROUBLESHOOTING.md). If that does not solve it, [open an issue](../../../issues/new/choose) and fill in the form. If the app closed unexpectedly, attach the `crash-log.txt` that appears next to the exe.
