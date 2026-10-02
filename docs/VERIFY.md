# Verify your download

The app is not code-signed, so Windows cannot tell you who published it. These checks let you confirm that the zip you have is the one released here. Do them before you run it.

## 1. Download from the right place

Only download from this repository's [Releases page](../../../releases). Do not run copies that someone else re-uploaded.

## 2. Check the SHA256

Every release lists the SHA256 of its zip in the release notes and in `SHA256SUMS.txt`. The current release's is:

```
0e3c31ac212c18b30f72d552d2db7c4558daf35a91d8b7aba1f6d984b88736d1  Leafs-Grand-Blue-Autofish-v0.1.0.zip
```

To check yours, open PowerShell in the folder with the zip and run:

```powershell
Get-FileHash .\Leafs-Grand-Blue-Autofish-v0.1.0.zip -Algorithm SHA256
```

The `Hash` it prints must match exactly. If it does not, delete the file and download it again.


## About "Windows protected your PC"

This SmartScreen screen appears for programs that are new or unsigned. Choose **More info**, check that the name is **Leaf's Grand Blue Autofish.exe**, and only then choose **Run anyway**. If you would rather not, you do not have to.

## What the app does once it runs

It looks at your screen and sends mouse and keyboard input to Roblox. It saves its files in its own folder and makes no network connections of its own, apart from the optional Microsoft runtime download described in the [privacy notice](../legal/PRIVACY.txt). To remove it, delete the folder.
