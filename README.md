# Silent Hill 3 for iPhone: build your own

Turn **your own copy** of Silent Hill 3 for PC into an iPhone app, all from your phone. GitHub builds it for free.

It runs natively (no emulator) with touch controls, 60 fps and controller support.

## What you need

- A free [GitHub account](https://github.com/signup).
- **Silent Hill 3 for PC** as **one file**: the game's ISO, or the installed game's folder (the one with
  `sh3.exe`) zipped (.iso, .zip, .7z or .rar).
- A way to install apps from outside the App Store (see [Installing](#installing)).
- About **8 GB** free on your iPhone.

## Make it

1. **Share your game.** Put the file in Google Drive (or Dropbox). In Drive: tap **⋮ > Share**, set
   **General access** to **Anyone with the link**, then **Copy link**.
2. **Make your copy of this page.** Tap the green **Use this template** button at the top, then **Create a new
   repository**. Any name, choose **Private** (your game goes in it), **Create repository**.
   *Don't see the button? In Safari, tap **aA > Request Desktop Website**.*
3. **Build.** In your copy: **Actions** > **Build Silent Hill 3 for iPhone** > **Run workflow**. Paste your link
   in the first box and tap the green **Run workflow**. It takes about 20–30 minutes; you can close the page.
   A green tick means done. A red cross: tap it to see what went wrong, in plain words.
4. **Get the app and game files.** On your copy's front page, scroll to **Releases**:
   - **Silent Hill 3 app**: tap **SH3.ipa** and install it (see below).
   - **Game files**: download every **SH3-game-N.zip**, then in the **Files** app move them from *Downloads* to
     **On My iPhone > Silent Hill 3**.
5. **Play.** Open the app. The first time, it unpacks the zips (a few minutes) and deletes them.

## Installing

| | Cost | Computer? |
|---|---|---|
| **[SideStore](https://sidestore.io)** | Free (your Apple ID) | Once, to set it up. After that, open SideStore and tap **Refresh All** at least once a week: if you go past 7 days, SideStore and your apps expire and you'll need the computer again. |
| **[Signulous](https://www.signulous.com)** or **[UDID Registrations](https://www.udidregistrations.com)** | About $20 a year | No. Upload the IPA to their site and install from there. |
| **[Feather](https://github.com/khcrysalis/Feather)** | Your own [Apple Developer account](https://developer.apple.com/programs/) ($99 a year), or a signing service's certificate | No |

<details>
<summary>More options and details</summary>

- **[AltStore](https://altstore.io)** and **Sideloadly** are free too, but need a computer every week or every
  install.
- **[AppDB PLUS](https://appdb.to)** (about €12 a year) works like Feather: it needs a developer account or
  certificate.
- UDID Registrations also gives you certificate files you can use in Feather.
- Signing services are third parties, not part of this project. Apple sometimes revokes their certificates; the
  app then won't open until the service re-signs it.
- With a free Apple ID, iOS gives apps less memory space than the game normally reserves, so it runs with a
  smaller amount (`guest arena` in its log). A paid developer account removes that limit.

</details>

## Updating

In your copy: **Actions** > **Build Silent Hill 3 for iPhone** > **Run workflow**, with the link box **empty**.
Only the app is rebuilt (about 15 minutes). Install the new SH3.ipa the same way; your game files and saves stay.

## Playing

- **Move:** a stick appears under your left thumb. Push past its ring to run.
- **Look:** drag on the right side.
- **FIRE**, **AIM**, **ACTION** at the bottom right (a quick tap on the right is ACTION too); **MAP**, **ITEMS**
  and the flashlight at the top left.
- **MENU** (top right): tap to pause or skip; hold for settings (look speed, opacity, 60/30 fps, resolution,
  photo camera, cheat, classic controls, free camera).
- Controllers (Xbox, PlayStation, MFi) work; the touch buttons hide while one is connected.
- Phone warm? Set **RATE** to 30 or **RES** to BAL in the settings.

## Good to know

- **Keep your copy private** and don't share the app or game files: they're made from your game.
- A free GitHub account's 2,000 monthly build minutes cover many builds; one uses under a tenth.
- Saves are in *Files > On My iPhone > Silent Hill 3 > savedata*.
- Problems? The app writes `sh3.log` (and `sh3-crash.log` after a crash) in the same Files folder.

## Credits

- **[cutarev](https://github.com/cutarev/sh3-nx)**: the Silent Hill 3 port, the PC game turned into native code.
- **[sithewok13-dev](https://github.com/sithewok13-dev/sh3-nx/tree/ios)**: the iPhone version, touch controls and
  this template.

Silent Hill is a trademark of Konami. Not affiliated with or endorsed by Konami. This project contains nothing of
the game: you build from your own copy.
