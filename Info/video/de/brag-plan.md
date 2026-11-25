# Brag Plan: Rotor Display

## What is this app?
ESP32-S3 firmware (v1.5.9) for a round knob display that points an antenna rotor: azimuth, elevation, antenna choice and wind on one 466×466 face.

## The angle
A very large, very distant object obeys one small knob. Calm instrument-film delivery, dry last line. German edition: on-screen text and narration in German; voice is Piper de_DE-thorsten-high because Kokoro has no German voice.

## Hook (first 2-3 seconds)
Pale sky, black roof, a Yagi antenna. "Sie ist da oben." Then, inside the dark of the house: "Du bist hier unten." beside a tiny glowing ring.

## Key moments
- Camera dives into the tiny ring, which becomes the instrument.
- Real boot: Initialisiere → Referenziere (orange chase, 70 ms per LED) → Betriebsbereit (16 LEDs green, red direction dot).
- Knob: 0.1° per click (encoder_delta 1). T climbs; after the idle pause A and the antenna follow.
- Long press (450 ms): compass becomes the Elevation dial.
- Swipe: KW Beam / 2m / 70cm / 23 cm, then wind 33.4 kmh, 25.1 °C (the UI's own placeholder values).

## Outro / punchline
Back out to the roof. The antenna has turned. "Rotor Display — Auf den Punkt."

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
See share-copy.txt.

## Audio direction
- Role: warm bed under narration, sparse motion-matched accents
- Music: happy-beats-business-moves-vol-10 (110 BPM), CC BY 4.0
- Music treatment: 0.13 under voice, lifts in the gaps and after the last line, fade at the end
- Music cue guidance: bundled preset; strong cues 15.82, 18.55, 20.19; beats 6.82, 15.28, 17.47
- Audio-reactive treatment: subtle; LED spill on the ground breathes with RMS
- SFX posture: sparse; knob clicks, button, tap, swipes, one landing bell
- Restraint rule: nothing competes with a spoken word

## Voiceover script (Piper de_DE-thorsten-high)
1. 0.25 — Auf dem Dach steht eine Antenne. Hier sagst du ihr, wohin sie schauen soll.
2. 4.45 — Es wacht auf, sucht die Referenz und wird grün, sobald es bereit ist.
3. 8.95 — Dreh am Knopf. Jeder Klick ist ein Zehntelgrad. Hör auf zu drehen, und der Rotor folgt.
4. 14.50 — Taste halten, und aus Azimut wird Elevation.
5. 17.85 — Drei Antennen. Wind live.
6. 20.95 — Rotor Display. Auf den Punkt.

## Storyboard
### Scene 1 — Roof — 4.1s
Sky, roof, antenna, cable to a tiny ring. "Sie ist da oben." / "Du bist hier unten." Audio: music opens, voice. Transition: continuous dive into the ring.
### Scene 2 — Boot — 4.2s
Device centred; three status messages, ring follows firmware states. Sequential: yes, status messages one by one. Ready lands on beat 6.82. Transition: device slides left.
### Scene 3 — Knob — 5.9s
Device left, plan-view antenna right. Interaction: knob turns, T climbs in tenths, A + antenna follow. "0,1° pro Klick".
### Scene 4 — Elevation — 3.2s
Interaction: 450 ms hold, toggles on beat 15.28. Side-view antenna tilts. "Halten: AZ → EL".
### Scene 5 — Antennas, wind — 2.7s
Interaction: swipe, tap "2m / 70cm" (18.55 strong cue), swipe to wind.
### Scene 6 — Roof again — 4.2s
Pull-out on strong cue 20.19; antenna swings round and tips up. Title, then "Auf den Punkt." held 2 s.

**Music mood:** upbeat but low. **Audio summary:** voice leads, bed supports, bell lands the pun.
