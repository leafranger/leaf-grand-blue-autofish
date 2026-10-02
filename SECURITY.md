# Security

## Reporting a problem

If you find a security problem in Leaf's Grand Blue Autofish, please **do not open a public issue**. Write to **leafrangerit@gmail.com** with what you found and how to reproduce it. You will get a reply as soon as it can be read; this is a one-person project, so please be patient.

For ordinary bugs, use the [issue form](../../issues/new/choose).

## What the app does and does not do

- It runs on your PC and needs no account.
- It takes pictures of your screen, reads them, and sends mouse and keyboard input. It does not read or change Roblox's files or memory.
- It makes no network connections of its own. The one optional exception: if your PC lacks Microsoft's Visual C++ runtime, the first start can download Microsoft's official installer **only if you click to allow it**; the file's signature is checked as Microsoft's before it is run.
- It saves its files (settings, calibration, sessions) in its own folder. Optional debug pictures of the game window are only saved if you turn them on.
- It is not code-signed. [Verify your download](docs/VERIFY.md) before running it.

## Supported versions

Only the latest release receives fixes.
