# Security

## Reporting a problem

If you find a security problem in Leaf's Grand Blue Autofish:

1. **Report it on [Discord](https://discord.gg/AC8qRsUHsc) first.** That is where it gets seen fastest. If it is sensitive, say you have a security problem and ask to talk privately instead of posting the details in a public channel.
2. **Email only if that does not work** (no answer, or it cannot wait): **leafrangerit@gmail.com**, with what you found and how to reproduce it.

Please do not post details of a security problem in a public GitHub issue. Public issues are read less often than Discord.

For ordinary bugs, ask on Discord or use the [issue form](../../issues/new/choose).

## What the app does and does not do

- It runs on your PC and needs no account.
- It takes pictures of your screen, reads them, and sends mouse and keyboard input. It does not read or change Roblox's files or memory.
- It makes no network connections of its own. The one optional exception: if your PC lacks Microsoft's Visual C++ runtime, the first start can download Microsoft's official installer **only if you click to allow it**; the file's signature is checked as Microsoft's before it is run.
- It saves its files (settings, calibration, sessions) in its own folder. Optional debug pictures of the game window are only saved if you turn them on.
- It is not code-signed. [Verify your download](docs/VERIFY.md) before running it.

## Supported versions

Only the latest release receives fixes.
