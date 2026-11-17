# Zeekret Dash: Automation guide

When something happens on the car, Zeekret Dash does what you picked. Each rule reads
"**When** … **only if** … **do** …".

[Back to the README](../../README.md) · [Changelog](../../CHANGELOG.md)

## Getting started
1. Tap the **Automation** card on Home and turn on the main switch (rules only run while it's on).
2. Tap **Add rule**, pick a **When**, an optional **Only if**, and at least one **Do**.
3. Tap **Try it now** to run the rule's actions straight away. **Test parked first.**
4. Each rule can be switched on or off, edited or deleted.

## When
- The car is switched on / off
- Shift to P / D / R
- Speed **reaches** or **drops to** a number, or **enters** / **leaves** a range (0–200 km/h in 5 km/h steps)
- Outside temperature **rises to** or **drops to** a number
- It gets dark / it gets light
- Rain starts / rain stops

## Only if (optional)
- Days: workdays or the weekend
- Gear: in P / D / R
- Light: when dark / when light
- Rain: while raining / while dry
- Speed: above / below / between
- Outside temperature: above / below

## Do (in order)
- **Car controls:** acceleration mode, steering, damping (Performance trim only), sunroof shade, rear fog light,
  low-speed emergency braking, air conditioning, temperature zones, tailgate opening height.
- **App actions:** Blindspot camera on / off, show it on HUD / head unit / both, rearview mirror open / close,
  mirror view, mirror anti-glare, night dimming, dash cam on / off.

## No flickering
- A rule runs on a **change**, not on a state. "The car is switched on" runs when the car goes from off to on.
- A speed or temperature rule only runs again after the value has moved back past its number first
  (5 km/h for speed, 1 °C for temperature).
- Speed and rain rules run at most once every 30 seconds, temperature rules once every 60 seconds.

## Examples
| You want | When | Only if | Do |
|---|---|---|---|
| Sportier on the expressway | Speed reaches 90 km/h | | Acceleration mode: Sport |
| Softer back in town | Speed drops to 60 km/h | | Acceleration mode: Comfort |
| Be seen in the rain | Rain starts | When dark | Rear fog light: On |
| No glare at night | It gets dark | | Mirror anti-glare: High, Night dimming: On |
| Mirror away when parked | Shift to P | | Rearview mirror: Close |
| Towing a trailer | Car switched on / speed reaches 10 km/h | | Low-speed emergency braking: Off (the **Trailer mode** card sets these up for you) |

> The car always has the last word: some commands only work in some states (for example, the rear fog light only
> works while the headlights are on).
