# Verify your download

The app is not code-signed, so Windows cannot tell you who published it. These checks let you confirm that the zip you have is the one released here. Do them before you run it.

## 1. Download from the right place

Only download from this repository's [Releases page](../../../releases). Do not run copies that someone else re-uploaded.

## 2. Check the SHA256

Every release lists the SHA256 of its zip in the release notes and in `SHA256SUMS.txt`. The current release's is:

```
54b8fa6de1fa26a43c25b3e1d2cbaff2648f08a3a0f3cc59352357d571e187b6  Leafs-Grand-Blue-Autofish-v0.1.1.zip
```

To check yours, open PowerShell in the folder with the zip and run:

```powershell
Get-FileHash .\Leafs-Grand-Blue-Autofish-v0.1.1.zip -Algorithm SHA256
```

The `Hash` it prints must match exactly. If it does not, delete the file and download it again.

## 3. Check the antivirus scan

The program inside the zip, `Leaf's Grand Blue Autofish.exe`, was scanned with VirusTotal: [see the result](https://www.virustotal.com/gui/file/bf76e87231cecfa6f2e16bff1c0f57c2b0e6c2509278e0f61d31135e7bf27417). Its SHA256 is:

```
bf76e87231cecfa6f2e16bff1c0f57c2b0e6c2509278e0f61d31135e7bf27417
```

Open the result and read it for yourself. If you want to be sure, compare the hash on the VirusTotal page with the one above.

## If an antivirus flags it

Antivirus programs sometimes flag a safe file. This is called a false positive, and it is likely for this app: it sends mouse clicks and listens for hotkeys, which is also what some unwanted software does, and it is new and unsigned, so security tools have little history to judge it by.

Usually you can ignore a flag when **all** of these are true:

- Only one or a few engines out of the many on VirusTotal flag it, not most of them.
- The name is generic or made from the file's hash (for example `Ti!` followed by letters and digits, `Heur`, `Generic`, `Suspicious`, `ML` or `Unsafe`) and not the name of a known malware family.
- The SHA256 of your zip matches the one above, so you know it is the file released here.

If many engines flag it, a named malware family appears, or your SHA256 does not match, do not run it: delete it and ask on the [Discord server](https://discord.gg/AC8qRsUHsc).

If your own antivirus blocks it, you can report it as a false positive to that vendor. You decide whether to trust the app.

## About "Windows protected your PC"

This SmartScreen screen appears for programs that are new or unsigned. Choose **More info**, check that the name is **Leaf's Grand Blue Autofish.exe**, and only then choose **Run anyway**. If you would rather not, you do not have to.

## What the app does once it runs

It looks at your screen and sends mouse and keyboard input to Roblox. It saves its files in its own folder and makes no network connections of its own, apart from the optional Microsoft runtime download described in the [privacy notice](../legal/PRIVACY.txt). To remove it, delete the folder.
