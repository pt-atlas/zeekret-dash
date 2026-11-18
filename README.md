# Zeekret Dash (head unit)

A head-unit app for the **Zeekr 7X**: a blindspot camera on the HUD and the centre screen when you indicate,
a digital rearview mirror, a 4-camera dash cam, car controls, automations, and the **battery % you'll arrive with**
while Google Maps navigates on your phone.

| App | Runs on | What it does |
|---|---|---|
| **[Zeekret](https://github.com/pt-atlas/zeekret-updates)** | Phone + Wear OS watch | Bluetooth digital key, remote control, stats, widget |
| **Zeekret Dash** (this one) | Car head unit | Everything below |
| **[Zeekret Maps Link](https://github.com/pt-atlas/zeekret-maps-link)** | Phone | Sends your live Google Maps route to Zeekret Dash for **battery at arrival** |

**Guides:** [Automation guide with examples](docs/guide/automation.md)

**⬇ Download:** open **[zeekret.pages.dev](https://zeekret.pages.dev/)** in the browser **on the car's head-unit
screen** and download **Zeekret Dash** (Experimental). Opening the link on a phone or computer won't install it on the car.
What changed in each version: [CHANGELOG.md](CHANGELOG.md).

> This repository holds **documentation only, no source code**. Zeekret Dash is closed-source.

> 🚗 **Tested on the Zeekr 7X only (SEA region).** Any other car or region is entirely at your own risk.

> 🧪 **Experimental, unofficial software** with no vehicle safety certification. It does not replace your mirrors,
> the factory 360° view, the reversing camera or the car's own blind-spot warning. Always look before you turn or
> change lane. Not affiliated with Zeekr, Geely or ECARX. Use at your own risk: no warranty, no responsibility for
> anything that happens from using it.

## Install

1. In the car's browser open **zeekret.pages.dev** and tap **Download** on Zeekret Dash.
2. Install it **through App Lab**, the way other 7X third-party apps are installed.
3. When the installer finishes, tap **Back** (top left), **not Open**. The head unit's installer can get stuck otherwise.
4. Open **Zeekret Dash**. Allow **Display over other apps**, **Camera** and **Notifications**.
5. Indicate: that side's camera appears. Cancel the indicator: it goes away.

Updates install over the old version and keep your settings and licence. Plug in a USB stick for the dash cam and the
settings backup. The car's own camera features (factory 360° view, reversing camera) always win: while they're on, a
picture may go black until they release the camera.

## Features and how to use them

### Home
A grid of cards, three wide. **Tap** a card to act, **hold** it to open its settings.

| Row | Cards |
|---|---|
| 1 | Blindspot camera · Show it on · Rearview mirror |
| 2 | Mirror view · Car's blindspot lamp · Night dimming |
| 3 | Dash cam · Automation · Trailer mode |
| 4 | Acceleration mode · Steering · Damping |
| 5 | Rear fog light · Battery at arrival · Licence |
| 6 | About |

The side menu: Home · Blindspot · Dash cam · Car · **Map link** · Automation · Licence · About.

On cars without adjustable damping (not the Performance trim) the Damping card stays in its place, greyed out and
marked **Not available**.

### Blindspot camera
Indicate, and the camera on that side appears. It goes away when the indicator stops. Hazards show nothing.
- **Show it on:** HUD (default), head unit, or both. Tap the card to switch.
- **When it's armed:** Always when armed (default) or Only while driving (in D).
- **Blindspot view:** the side camera's fisheye picture is straightened into a normal view, aimed along the side of
  the car toward the rear, and mirrored like a real mirror.
- **HUD pictures slide in** from the HUD's outer edge and slide out again (0.2 s). The HUD picture is sized to the
  part of the HUD you can actually see.
- **Head-unit panel:** Small / Medium (default) / Fullscreen, on the right side.
- **Blindspot ▸ Aim:** swing toward the rear, lift, level the horizon and view width, with a live preview.
- **Blindspot ▸ Display:** HUD view width, HUD transparency, and **Show border on the HUD (10 s)** to check where the
  picture sits.
- **Night dimming:** dims the panels at night, with its own night brightness. Tap the card to turn it on or off.

### Safety extras (Blindspot ▸ Camera ▸ Safety)
| Feature | What it does | Default |
|---|---|---|
| Stay up until the wheel is straight | If you cancel the indicator mid-turn, the camera stays until the wheel is straight again | On |
| Turn without indicator | Below 30 km/h, turning the wheel more than 90° without indicating shows that side | On |
| Forgot-to-indicate check | Above 60 km/h, a quick steering move without the indicator shows that side (Low / Medium / High) | On |
| Camera on the door-open warning | When the car warns that something is coming as a door is about to open, that side's camera shows | On |
| Car's blindspot lamp | When the lamp in the door mirror lights, that side's picture gets a blinking red edge; above 60 km/h the camera also opens without the indicator | On |

### Head-unit rearview mirror
A digital mirror over the head-unit screen. Turn it on with the **Rearview mirror** card; its button appears in D.
- **Mirror view** (tap the card, or long-press the mirror button):
  - **Rearview:** the rear camera as a mirror.
  - **Slide-in:** the rear picture in the middle; the left and right blindspot pictures slide in at the sides when
    they're needed.
  - **Blindspot** (default): both side pictures.
- Drag to move and pinch to resize at any time; the shape never changes. A **Reset** button shows for 5 s.
- **Night anti-glare:** Off / Low (default) / High. Calms bright headlights in the rear picture.
- Settings: translucency, Slide-in side zoom / height / angle and middle width, Blindspot zoom / height /
  inner ↔ outer, rear aim (tilt, view width, left / right), reset buttons.

### Dash cam
- Records **all four surround cameras** as one 2560 × 1440 picture while driving, in 1-minute clips.
- Saves to the **USB stick** (folder ZeekretDash) or the car's own storage. When space runs low, the oldest clips
  are deleted.
- Stamps **date, time and speed** into the video. Optional **.gpx location track** beside each clip (opens in
  Google Earth).
- **Protected clips:** a hard stop locks the current clip and the one before it. You can lock a clip by hand too.
  Locked clips are never deleted.
- **Playback** tab: browse, filter (all / locked only) and play clips, with a USB check and "where to find the
  clips" help.

### Battery at arrival (side menu ▸ Map link)
Shows the **battery % you'll arrive with** as one small line on the head unit (and / or the HUD):
**🔋 69% 🏁** for a destination, **🔋 62% 🏠** for home. **Orange** below 20 %, **red** below 5 %; if you won't make
it, **🔋 0%** in red. Tap the **Battery at arrival** card on Home to turn it on or off; hold it, or pick **Map link** in
the side menu, for its settings.

Where the destination comes from, first match wins:
1. **Live Google Maps route** from the phone app **[Zeekret Maps Link](https://github.com/pt-atlas/zeekret-maps-link)**:
   the exact km left on Google's route, updated every few seconds. Change the destination in Google Maps and the car
   follows. With stops, the % is for the final destination.
2. **A shared place:** in Google Maps on the phone tap a place ▸ **Share ▸ Zeekret ▸ Battery at arrival** (Zeekret
   phone app .60 or newer), or a **saved place** picked on the Map link page. Km left = the car's GPS straight-line
   distance × 1.3. It hides when you arrive (within 300 m).
3. **Home** ("This is home" on the Map link page): shown when you're more than 1 km away and nothing else is set.

How to set it up:
- **Link the phone:** the Map link page shows the car's **pair code** (like `ABCD-EFGH`) under *Link with the phone
  app*. Type the same code into Zeekret Maps Link and / or the Zeekret phone app (Settings).
- **Allow location** on the Map link page (needed for shared places and home).
- **Battery size:** 75 or 100 kWh. **Where it shows:** head unit, HUD or both.
- On the head unit, **drag** the panel to move it and **pinch** to resize it; a **Reset** button shows for 5 s.
- It hides while the car is in **P** and while a blindspot camera picture is showing.

How the % is worked out: with the car's average consumption (sent by the phone), battery % − km × kWh per 100 km ÷
battery size; without it, battery % × (range − km left) ÷ range. It's an estimate: keep an eye on the car's own range.

Privacy: the phone sends only km left, arrival time (and for a shared place, its position and name), **locked
(AES-256-GCM)** with a key only your phone and your car know. The server in between can't read it and deletes it
after 24 h.

### Car controls
On the **Car** page, and as Home cards for the main ones.

| Control | Choices | Note |
|---|---|---|
| Acceleration mode | Comfort / Normal / Sport | Changes at once, also while driving |
| Steering | Comfort / Standard / Sport | The car's Custom drive mode setting |
| Damping | Comfort / Standard / Sport | **Performance trim only.** The car doesn't report it, so the app shows the last choice it sent |
| Sunroof shade | Closed / 25 / 50 / 75 % / Open | The car decides when the shade may move |
| Rear fog light | On / Off | Only while the headlights are on |
| Low-speed emergency braking | On / Off | When off, the car won't brake for you at low speed |
| Air conditioning | On / Off | |
| Temperature zones | Same both sides / Separate | |
| Tailgate opening height | 50 – 100 % | How far the power tailgate opens |

**Find a car setting** (Car page, read-only): take a **snapshot**, change a setting in the car's own menu, then
**compare** to see which car value changed. **Search car signals** lists the car's signals by any words. Neither
changes anything on the car.

### Trailer mode
For towing, when the car's low-speed emergency braking would brake for the trailer behind you.
- **On:** switches low-speed emergency braking **off** now, every time the car is switched on, and again when the
  speed reaches 10 km/h (two automation rules, which also turns Automation on).
- **Off:** stops those rules. It does **not** switch the braking back on: do that on the Car page.
- Hold the card to see the rules on the Automation page.

### Automation
"**When** … **only if** … **do** …". Open the **Automation** card and turn it on. Full guide with examples:
[docs/guide/automation.md](docs/guide/automation.md).
- **When:** the car is switched on or off; shift to P, D or R; speed reaches or drops to a number, or enters or
  leaves a range (0–200 km/h in 5 km/h steps); outside temperature rises or drops to a number; it gets dark or
  light; rain starts or stops.
- **Only if** (optional): workdays or weekend; gear in P, D or R; dark or light; raining or dry; speed above, below
  or between; outside temperature above or below.
- **Do**, in order: any car control above, plus app actions: Blindspot camera on / off, show it on HUD / head unit /
  both, rearview mirror open / close, mirror view, mirror anti-glare, night dimming, dash cam on / off.
- **No flickering:** a rule runs on a change, not a state. A speed or temperature rule only fires again after the
  value has moved back past its number, and at most once every 30 s (speed, rain) or 60 s (temperature).
- **Try it now** runs a rule's actions straight away. Test car actions parked first.

### Settings backup on the USB stick
**About ▸ Settings backup** saves all settings and automation rules to the USB stick (ZeekretDash/Backup) and restores
them after a reinstall. The licence is not part of the backup and isn't needed: it stays with the car.

### Fault log
If something goes wrong, open **About ▸ Fault log** and send it for checking.

### Reliability
- Runs in the background, starts when the car starts, and restarts itself if it stops.
- One camera feed drives every picture at about 30 fps. A late picture keeps the last frame (amber edge);
  "NO SIGNAL" shows only after 1 s.

## Licence
A **7-day free trial**, then a paid licence per car (price and how to pay on the app's **Licence** page and at
zeekret.pages.dev). The licence is checked offline once issued, survives updates and reinstalls, and a reinstall
doesn't restart the trial. A licence can be revoked in case of misuse.

## Questions and problems
Open an [issue](../../issues) with what happened, the app version (About) and, if you can, the fault log.

---

© Zeekret Dash. All rights reserved. This repository contains documentation only; no source code is published.
