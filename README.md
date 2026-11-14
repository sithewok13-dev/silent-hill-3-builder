# Silent Hill 3 for iPhone: build your own

Make the iPhone app from **your own copy** of Silent Hill 3 for PC, entirely on your phone. GitHub's computers
do the building for free; you need no Mac or PC.

It runs the game natively (the PC game's code turned into iPhone code, no emulator), with touch controls made
for the phone, 60 fps, and controller support.

## What you need

- A free [GitHub account](https://github.com/signup).
- **Your copy of Silent Hill 3 for PC** as one file in Google Drive or Dropbox: the game's ISO, or the installed
  game's folder zipped (the one with sh3.exe; any of .iso, .zip, .7z, .rar). Share it as **Anyone with the link**.
- A way to install apps that aren't from the App Store (see **Installing** below): free with
  [SideStore](https://sidestore.io) (your normal Apple ID, and a computer once to set it up), or with no computer
  through a paid signing service (about $20 a year) or Feather with an Apple Developer account.
- About **8 GB** free on the iPhone (iOS 15 or later; an iPhone from 2020 or newer is best).

## Make it (4 steps, about 30 minutes, mostly waiting)

1. **Make your copy of this page.** Tap the green **Use this template** button above, then **Create a new
   repository**. Give it any name, choose **Private** (important: your game goes in it), and tap **Create
   repository**.
2. **Start the build.** In your new copy, tap **Actions**, then **Build Silent Hill 3 for iPhone** on the left
   (on a phone: the ☰ menu), then **Run workflow**. Paste the link to your game in the first box and tap the green
   **Run workflow**.
3. **Wait.** It takes about 20–30 minutes. A green tick means it's done; a red cross shows what went wrong in plain
   words when you tap it. You can close the page and come back.
4. **Install it.** Tap **Releases** on your copy's front page (on a phone: scroll down):
   - In **Silent Hill 3 app**, tap **SH3.ipa**, then open it with SideStore, your signing service or Feather.
   - In **Game files**, download every **SH3-game-N.zip**. Then in the **Files** app, move them from
     *Downloads* to **On My iPhone > Silent Hill 3** (that folder appears once the app is installed).

Start the app. The first time, it unpacks the zips (a few minutes, with a progress bar) and then deletes them.

## Installing

The app isn't from the App Store, so your iPhone needs a sideloading app to install it. Pick one:

| | Cost | Computer needed? | Good to know |
|---|---|---|---|
| **[SideStore](https://sidestore.io)** (easiest free one) | Free, your normal Apple ID | Once, to set it up | Apps last 7 days; open SideStore and tap **Refresh** to renew them. Up to 3 apps. |
| **[AltStore](https://altstore.io)** | Free | Yes, every week (AltServer) | Apps last 7 days |
| **Sideloadly** | Free | Yes, each install | Apps last 7 days |
| **A signing service**: [Signulous](https://www.signulous.com) or [UDID Registrations](https://www.udidregistrations.com) | About $20 a year | No | Upload the IPA to their site and install it from there. UDID Registrations also gives you certificate files that work in Feather. Third-party services, not affiliated with this project; Apple sometimes revokes their certificates, and then the app stops opening until the service re-signs it. |
| **[Feather](https://github.com/khcrysalis/Feather)** (or [AppDB PLUS](https://appdb.to), about €12 a year) | Needs your own **paid Apple Developer account** ($99 a year) or a signing service's certificate files | No | Install with that certificate; apps last as long as it does. |

With a free Apple ID, iOS gives apps less memory space than the game normally reserves; the app then runs with a
smaller amount (see `guest arena` in its log). A paid Apple Developer account removes that limit.

## Updating the app

When the port gets new features: in your copy, tap **Actions > Build Silent Hill 3 for iPhone > Run workflow**,
leave the link **empty**, and run it. Only the app is rebuilt (about 15 minutes); install the new SH3.ipa the same way
as before. Your game files and saves stay as they are.

## Playing

- **Move:** a stick appears wherever your left thumb lands. Push past its ring to run, any direction.
- **Look:** drag on the right side. With **VIEW** set to FREE in the settings, a camera behind Heather follows your
  drag instead of the game's fixed cameras.
- **FIRE**, **AIM** and **ACTION** at the bottom right; a quick tap anywhere on the right is ACTION too.
- **MAP**, **ITEMS** and the flashlight at the top left.
- **MENU** (top right): tap to pause or skip; hold it to open settings (look speed, button opacity, 60 or 30 fps,
  resolution, a photo camera with selfies, a cheat, classic controls, fixed or free camera).
- A controller (Xbox, PlayStation, MFi) works too; the touch buttons hide while one is connected.
- If your phone gets warm, set **RATE** to 30 or **RES** to BAL in the settings.

## Good to know

- **Keep your copy private.** It holds your game. Don't share the app or the game files you make.
- **Free minutes:** a free GitHub account comes with 2,000 build minutes a month for private copies. A first build
  uses about a quarter of them; an update, less.
- **The game's own saves** live with the game files, in *On My iPhone > Silent Hill 3 > savedata*.
- **If something goes wrong:** the app writes `sh3.log`, and `sh3-crash.log` after a crash, in its Files folder.

## Credits

- **[cutarev](https://github.com/cutarev/sh3-nx)**: the Silent Hill 3 port, the PC game turned into native code.
- **[sithewok13-dev](https://github.com/sithewok13-dev/sh3-nx/tree/ios)**: the iPhone version, touch controls and
  this template.

Silent Hill is a trademark of Konami. This project is not affiliated with or endorsed by Konami, and it contains
nothing of the game: you build from your own copy.
