# Brag Plan: Rotor Display

## What is this app?
ESP32-S3 firmware (v1.5.9) for a round knob display that points an antenna rotor: azimuth, elevation, antenna choice and wind on one 466×466 face.

## The angle
A very large, very distant object obeys one small knob. Calm instrument-film delivery, dry last line. German UI stays German (verbatim from the firmware); narration is English because Kokoro has no German voice.

## Hook (first 2-3 seconds)
Pale sky, black roof, a Yagi antenna. "It's up there." Then, inside the dark of the house: "You're down here." beside a tiny glowing ring.

## Key moments
- Camera dives into the tiny ring, which becomes the instrument.
- Real boot: Initialisiere → Referenziere (orange chase, 70 ms per LED) → Betriebsbereit (16 LEDs green, red direction dot).
- Knob: 0.1° per click (encoder_delta 1). T climbs; after the idle pause A and the antenna follow.
- Long press (450 ms): compass becomes the Elevation dial.
- Swipe: KW Beam / 2m / 70cm / 23 cm, then wind 33.4 kmh, 25.1 °C (the UI's own placeholder values).

## Outro / punchline
Back out to the roof. The antenna has turned. "Rotor Display — Point taken."

## User flow worth showing
Boot and reference → turn the knob → antenna arrives → switch axis.

## Tone
- Preset: polished
- Creative direction: quiet instrument film with one dry pun
- Interpretation: one continuous take, few words, long holds, no hype

## Format: landscape — 1920x1080, 30 fps
## Duration: 24.3 s

## Visual identity (from the project)
- Background: #15171A (LVGL dark theme); sky #C9D3D8 for the outside world
- Accent: #2196F3 (arc, buttons); LEDs rgb(0,200,0) / rgb(255,0,0) / rgb(255,80,0); button on #087321
- Text: #FAFAFA on dark, #15171A on sky
- Display/body font: Montserrat (the firmware's LVGL font)
- Strongest visual element: compass face inside the 16-LED ring

## Privacy
No author names, callsigns, repository URLs or device addresses on screen.

## Share copy (draft)
There's an antenna on the roof. There's a knob on the desk. Rotor Display 1.5.9: 0.1° per click. Point taken.

## Audio direction
- Role: warm bed under narration, sparse motion-matched accents
- Music: happy-beats-business-moves-vol-10 (110 BPM), CC BY 4.0
- Music treatment: 0.13 under voice, lifts in the gaps and after the last line, fade at the end
- Music cue guidance: bundled preset; strong cues 15.82, 18.55, 20.19; beats 6.82, 15.28, 17.47
- Audio-reactive treatment: subtle; LED spill on the ground breathes with RMS
- SFX posture: sparse; knob clicks, button, tap, swipes, one landing bell
- Restraint rule: nothing competes with a spoken word

## Voiceover script (Kokoro af_heart)
1. 0.50 — There's an antenna on the roof. This is how you tell it where to look.
2. 4.60 — It wakes up, finds its reference, and goes green when it's ready.
3. 8.70 — Turn the knob. Every click is a tenth of a degree. Stop turning, and the rotor follows.
4. 14.50 — Hold the button, and azimuth becomes elevation.
5. 17.80 — Three antennas. Live wind.
6. 20.95 — Rotor Display. Point taken.

## Storyboard
### Scene 1 — Roof — 4.1s
Sky, roof, antenna, cable to a tiny ring. "It's up there." / "You're down here." Audio: music opens, voice. Transition: continuous dive into the ring.
### Scene 2 — Boot — 4.2s
Device centred; three status messages, ring follows firmware states. Sequential: yes, status messages one by one. Ready lands on beat 6.82. Transition: device slides left.
### Scene 3 — Knob — 5.9s
Device left, plan-view antenna right. Interaction: knob turns, T climbs in tenths, A + antenna follow. "0.1° per click".
### Scene 4 — Elevation — 3.2s
Interaction: 450 ms hold, toggles on beat 15.28. Side-view antenna tilts. "Hold: AZ → EL".
### Scene 5 — Antennas, wind — 2.7s
Interaction: swipe, tap "2m / 70cm" (18.55 strong cue), swipe to wind.
### Scene 6 — Roof again — 4.2s
Pull-out on strong cue 20.19; antenna swings round and tips up. Title, then "Point taken." held 2 s.

**Music mood:** upbeat but low. **Audio summary:** voice leads, bed supports, bell lands the pun.
