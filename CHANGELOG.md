# Changelog

Zeekret Dash for the Zeekr 7X head unit. Download the latest from **[zeekret.pages.dev](https://zeekret.pages.dev/)** on the car's screen.

## Zeekret Dash 1.26
- Everything from 1.25 beta 1: HUD **traffic bar of the next 50 km** (with Zeekret Maps Link 1.4.1), only the battery %
  coloured, time left **1 h 25 m**.
- Head-unit battery panel: default spot **0.5 cm lower** (every car moves to it once; Reset goes there).

## Zeekret Dash 1.25 betas
- **1.25.beta1:** HUD battery panel line 3 = a small coloured **traffic bar of the next 50 km** (blue clear, orange slow,
  red jam; white dot = your car), from Zeekret Maps Link 1.4 (Android 16 phone, Google Maps navigating). Only the battery
  % turns orange / red when low. Time left over an hour reads **1 h 25 m**.

## Zeekret Dash 1.25
- **Link by QR:** Map link (side menu) shows the pair code as a QR. The Zeekret phone app (.64) and Zeekret Maps Link
  (1.3) link to the car by scanning it (**Scan car code**), no typing. **New code** breaks every link at once.
- Everything from the 1.24 betas below: HUD time left, and the car licence + Renew on the linked Zeekret phone app.

## Zeekret Dash 1.24 betas (pre-release)
- **1.24.beta1:** HUD battery panel line 1 shows the time left next to the arrival time: **🏁 08:25 · 18 min**
  (**1 h 25** over an hour). Only with a live Google Maps route (Zeekret Maps Link).
- **1.24.beta2:** the car can be linked to the Zeekret phone app (type the car's pair code in Zeekret ▸ Settings ▸
  Zeekret Dash; Zeekret .63 or newer). The phone then shows this car's licence with a **Renew** button. Only a one-way
  hash of the pair code is sent, never the code itself.

## Zeekret Dash 1.24
- **Lane keep assist** On / Off: new car control on the Car page and as an Automation action ("Then").
- HUD battery panel: **arrival time on top** (🏁 08:25), battery % and km below (🔋 43% · 12 km), 5 mm higher.
- New defaults (fresh install and the Reset buttons; your saved settings stay): mirror view **Slide-in**; Slide-in side
  zoom 110 %, side height 6°; Blindspot mirror zoom 67 %, inner ↔ outer 0°; Aim (left / right) swing 45°, lift 11°,
  view width 135 %.
- Includes the 1.23 betas: battery panel on the head unit further left and 6 % bigger.

## Zeekret Dash 1.23 betas (1.23.beta1 – beta5)
- Battery at arrival panel on the head unit: default spot about 9.4 cm further left than 1.23 (same height), text and
  icons 6 % bigger. Every car moves to the new spot and size once after updating; Reset goes there from then on.

## Zeekret Dash 1.23
- Battery at arrival panel on the head unit: **one fixed default spot** (lower right, just left of the mirror button).
  Moving or resizing the rearview mirror no longer moves it, and **Reset** always puts it back there. A spot you
  dragged it to yourself stays until you tap Reset.
- Battery at arrival icon follows the shown %: 🔋 21–100 %, 🪫 orange 1–20 %, 🪫 red with a red glow at 0 %
  (head unit and HUD).

## Zeekret Dash 1.22 betas (1.22.beta12 – beta30)
- New **Nearby Charger** card: suggests the 3 nearest fast chargers (120 kW+) when the car is switched on below 30 %
  and when the battery drops to 30 %. Needs charger search switched on in the licence (greyed out, "Licence required",
  otherwise). The suggestions card stays until ✕, updates distances while driving and searches again after 10 km.
- Automation: battery triggers (**battery rises / drops to %**), battery condition (**above / below %**) and a
  **Suggest chargers** action.
- **Trailer mode** also switches the mirror to Blindspot; Off puts back the view you had.
- Home: row 4 Acceleration mode · Steering · Damping, row 5 Nearby Charger · Battery at arrival · Rear fog light.
  Licence and About moved to the side menu only.
- Battery at arrival on the HUD: two centred lines, **🔋 76% 🏁** and **23.4 km · 07:24**, no background, placed
  higher; stays up while driving (also over a blindspot picture). Default **Show on: Both**.
- The licence refreshes when you open the app (at most once a minute).

## Zeekret Dash 1.22 betas (1.22.beta1 – beta11)
- Side menu: new **Map link** item (the Battery at arrival settings) between Car and Automation.
- Battery at arrival panel: placed just left of the mirror button by default, no background; % text bigger, icons smaller.
- Tried and removed: showing the panel only while Android Auto is on screen (the head unit doesn't allow it).

## Zeekret Dash 1.22
- Battery at arrival panel without a background (just the icon and the number).
- New defaults: mirror view **Blindspot**; Aim (left / right) horizon 26°, swing 46°, lift 6°, view width 130 %.

## Zeekret Dash 1.21
- New app icon. Battery at arrival panel: new default place, size and look.

## Zeekret Dash 1.20
- Battery at arrival panel is one short line: **🔋 69% 🏁** (🏠 for home, red 0 % when you won't make it). Twice as
  big, hidden in P.

## Zeekret Dash 1.19
- Battery at arrival **live from Google Maps** with the new phone app Zeekret Maps Link: exact km left and arrival time,
  follows every destination change. **Home** and **saved places** (the last 10 shared). Clear destination.

## Zeekret Dash 1.18
- Battery at arrival from a **place shared from Google Maps** on the phone (Share ▸ Zeekret ▸ Battery at arrival). The
  destination is end-to-end encrypted. Asks for location.

## Zeekret Dash 1.17
- New **Battery at arrival** card and page: the battery % you'll arrive with, on the head unit and / or the HUD. Drag to
  move, pinch to resize. Orange below 20 %, red below 5 %.

## Zeekret Dash 1.16
- Home: on cars without adjustable damping (not the Performance trim) the Damping card stays in its place, greyed out
  and marked "Not available"; tapping it only explains why.

## Zeekret Dash 1.15
- Home order: row 3 Dash cam, Automation, Trailer mode; row 4 Acceleration mode, Steering, Damping.

## Zeekret Dash 1.14
- New **Trailer mode** card: On switches low-speed emergency braking off now, at every car start and at 10 km/h;
  Off stops those rules.
- Car page: **Low-speed emergency braking** On / Off.
- Smoother HUD drawing is always on. HUD picture size and height are fixed to fit the visible HUD area.
- New defaults: mirror view Slide-in; Blindspot mirror height and inner / outer 10°.

## Zeekret Dash 1.13
- Smoother HUD: pictures are drawn straight onto the HUD. HUD picture height setting.

## Zeekret Dash 1.12
- HUD picture size setting. Head-unit mirror: drag and pinch any time, the shape never changes, Reset button for 5 s.

## Zeekret Dash 1.11
- USB folder renamed ZeekretDash, backups in ZeekretDash/Backup. No freeze when the HUD picture hides.

## Zeekret Dash 1.10
- HUD border kept inside the visible area. More detail in the fault log.

## Zeekret Dash 1.09
- Damping shows only on cars that have adjustable damping (Performance trim).

## Zeekret Dash 1.08
- Car page ▸ Find a car setting: **Search car signals** by any words (read-only).

## Zeekret Dash 1.07
- **Settings backup / restore** on the USB stick (all settings and automation rules).

## Zeekret Dash 1.06
- **Damping** works (Comfort / Standard / Sport). Automation: Only if gear in P / D / R.

## Zeekret Dash 1.05
- Steering Comfort / Standard match the car. Drive mode renamed Acceleration mode.
- Automation: outside temperature triggers and conditions; speed 0–200 km/h in 5 km/h steps.
- No short HUD / mirror freeze when the camera restarts.

## Zeekret Dash 1.04
- Car controls match the car's Custom drive mode. Home: Damping and Acceleration cards.

## Zeekret Dash 1.03
- Car page: list suspension and drive-mode signals (read-only).

## Zeekret Dash 1.02
- New app icon. Car page ▸ **Find a car setting**: snapshot, change a setting in the car's menu, compare.

## Zeekret Dash 1.01
- Fixes: the app no longer closes when changing tabs after Aim; the Car page no longer redraws in a loop.

## Zeekret Dash 1.00
- First **Zeekret Dash** release. New **Home** screen of cards; Blindspot is one section (Camera / Display / Aim).
- **Car page:** drive mode, steering, sunroof shade, rear fog light, AC, temperature zones, tailgate height.
- **Automation:** "When … only if … do …" rules.
