# Hyperframes Composition Brief: Rotor Display

Objective: 24.3 s launch-style video. Composition `Info/video/en/composition/`, output `Info/video/en/brag.mp4`, 1920×1080, 30 fps.

Source: `src/ui/screens.c` (layout), `src/signals_ring_app.cpp` (ring states), `src/main.cpp` (knob, long press), `src/rotor_error_app.cpp` (status text), `data/img/*.png` (dial faces, wind arrow).
Verbatim copy: Initialisiere, Referenziere, Betriebsbereit, T, A, KW Beam, 2m / 70cm, 23 cm, kmh, °C, Elevation.

Creative contract: `brag-plan.md`. One continuous take, so one file rather than one sub-composition per scene; the device is the same object throughout.
LOOK: ground #15171A, sky #C9D3D8, accent #2196F3, Montserrat 500/700; dial redrawn as vector from Kompass_V5.png for sharpness at 1.4×.
BANNED: gradients, particles, floating loops, SaaS language, invented features, waveforms.

Audio: narration clips on their own lane, music ducked through a volume lane, SFX on one lane. LED spill is audio-reactive (RMS).
Beat locks: 6.82 ready, 15.28 axis toggle, 17.47 swipe, 18.55 tap, 20.19 pull-out.
Gate: `npx hyperframes check`.
