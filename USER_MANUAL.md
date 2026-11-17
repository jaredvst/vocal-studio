# Vocal Studio — User Manual

Vocal Studio is a complete vocal chain in one plugin: calibration, gate, de-esser, drive, compressor, tone EQ, focus, two effect slots, delay and reverb. Every module has **one main knob** for fast results and an **Advanced** panel (the `⋯` button) for full control.

Works on single leads (mono track) and on stacks/doubles (stereo track).

---

## Quick start

1. Insert Vocal Studio on a vocal track.
2. Press **LEARN** in the INPUT card and play about 4 seconds of singing. The ring turns **green** when the level is right. You can also set **Sensitivity** by hand until the ring is green.
3. Pick a preset from the header, or turn the main knobs: Gate **Threshold**, De-esser **Amount**, Compressor **Compress**, and so on.
4. Use **A/B** to compare two settings. Auto Gain keeps the output as loud as the input, so the comparison is fair.

> Sensitivity is never saved in presets. Presets therefore behave the same whether your recording is quiet or loud.

---

## The signal chain (fixed order)

Input / Sensitivity → Gate → De-esser (pre) → Drive → Compressor → Tone EQ → Focus → De-esser (post) → SFX 1 → SFX 2 → Delay + Reverb (sends) → Output

A shared **voice detector** tells the modules when you are singing, when it is an "s"/breath, and when it is silence:
- the gate stays open through word endings;
- the de-esser spares bright vowels;
- the delay and reverb duck under your voice;
- the pitch effects only act on sung notes.

---

## The screen

**Header:** presets (one list grouped into sections; ◀ ▶ to step, `*` = modified), Save / Delete (user presets), **A / B** and **copy**, **undo / redo** (also Ctrl+Z / Ctrl+Y), window size (70–100 %).

**Looks** (header menu; remembered on this computer; sound and settings are not affected):
- **Hardware Dark** (default): charcoal powder-coated faceplate, black knurled knobs with lit rims, red LED power switches, segment meters.
- **Desk Unit**: a photoreal hardware unit on a wooden desk: ivory chassis with bevelled edges and a cast shadow, slate knobs with printed dot scales, LED push-keys, red LED readouts for the selectors and a glass-fronted frequency screen.

**Frequency display + Tone EQ:**
- **Spectrum:** grey = input, amber = output. **DELTA** shows only what the chain changes (output − input).
- **Yellow nodes 1–5 (Tone EQ):** drag for frequency/gain, **mouse wheel** for Q (width), **double-click** to reset to 0 dB, **right-click** to switch a band on/off. Clicking a node selects it in the EQ strip.
- **EQ strip** (directly under the graph): EQ on/off, **Curve…** presets, Amount, Character, HP (with slope) / LP, band selector 1–5, and the selected band's On / Freq / Gain / Q / Type.
- **Blue handle (HPF):** drag the frequency. **Scroll on it to change the slope**: 12, 24, 36, 48 dB/oct or **Brickwall** (96 dB/oct). The curve redraws as you scroll. Double-click to switch it on/off.
- **Purple handle (De-esser):** drag the frequency; the purple curve dips live as it works. The dashed line shows the deepest possible cut.
- **Teal band (Focus):** shows where Focus is working and how much it lifts right now.
- **EQ HP / LP** handles appear when the EQ's high-/low-pass are switched on (scroll on HP for its slope).

**Modules:** each card has a power switch, its main knob, its key selector and meters. **Click a card** to show its **full controls** in the panel at the bottom (controls already on the card are not repeated there).

**Effects rack:** **+ ADD EFFECT** adds an effect, up to **6**. They run in order 1 → 6. Each tile has on/off, the effect type, Amount, **ADV** (its full controls) and **✕** (remove). The full controls also have **◀ earlier / later ▶** to reorder. Presets remember the rack.

**Help bar** (bottom line, **TIPS ON/OFF** button on the right): hover over any knob, button, handle, or **any option in a list** to see what it is and when it's typically used. For example, hovering *Vari-mu* in the compressor list explains vari-mu compression.

**Knobs:** drag up/down (Shift = fine), mouse wheel, **double-click** = default, **right-click** = **preset lock** 🔒. A preset-locked knob keeps its value when you load a different preset (for example, lock your compressor settings and browse tones). You can still turn it yourself; right-click again to unlock.

---

## Modules

| Module | Main knob | What it does | Advanced |
|---|---|---|---|
| **Input** | Sensitivity | Sets the input level to the −18 dBFS reference that all other modules are tuned for. LEARN sets it automatically. | HPF (on, freq, slope 12–48 dB/oct or Brickwall), stereo link |
| **Gate** | Threshold | Gently turns down noise between phrases (expander, not a hard mute). The **scope** shows level in (grey), level out (amber) and what is removed (**red**). Drag the white line to set the threshold. | Range, ratio, attack, hold, release, hysteresis, breath (how much breath passes), voice aware, sidechain HPF |
| **De-esser** | Amount | Tames "s/sh/t" with a dynamic high shelf. Two stages: Pre (before Drive, sees 5 ms ahead) and Post (after EQ/Focus). **LISTEN** plays only what is removed. | Freq, range, Pre↔Post, attack, release, mode (Split / Wide / Shelf), stages, S-only |
| **Drive** | Drive | 11 types: Transistor A, Triode, Pentode, Germanium, Console, Tape, Diode, Op-amp Clip, Fuzz, Exciter, Lo-fi. Auto Gain keeps the level steady while you add drive. Oversampled. | Tone, bias (even/odd), mix, output, lo-fi bits/rate |
| **Compressor** | Compress | Two stages in one knob: a slow **leveler** evens out phrases, and a fast **peak** stage catches spikes. 6 characters: FET, Opto, VCA, Vari-mu, Modern, Gritty. | Sensitivity (threshold offset), ratio (Auto/1.2–20), attack scale, release (Auto/ms), knee, Leveler↔Peak, **Upward** (lifts quiet sung words only, never the room noise), mix (parallel), SC HPF, makeup (auto + trim) |
| **Tone EQ** | Amount | 5-band EQ plus HP and LP. **Amount** scales the whole curve (50 % = half as strong). The **curve…** menu loads tone presets: Clarity, Warmth, Air Lift, De-mud, Presence, Radio Ready, Thin (Stacks), Dark & Smooth. | All band freqs/gains, band 1/5 Bell/Shelf, HP slope 12/24/48, Clean/Vintage character |
| **Focus** | Focus | A "make it pop" band (Body, Edge, Presence, Air or Custom). It lifts the region more when it is weak and less when it is already strong. | Region, custom freq/Q, voiced only |
| **Effects rack** | Amount (per effect) | Up to 6 of the 22 effects below, in series. Choosing a type sets its controls to good defaults. | P1–P4 (labels change per effect), mix, sync + division, wet HP/LP |
| **Delay** | Send | Patterns: Mono, Slap, Ping-pong, Wide. Colours: Clean, Tape, Bucket, Drum Echo. The power switch gates the **send**, so tails ring out. | Time / sync + division / **TAP**, feedback, width, drift, mod, ducking, HP/LP, → Reverb, duck attack/release/source |
| **Reverb** | Send | Room S/L, Chamber, Plate, Hall S/L, Gated, Reverse, Shimmer. | Size, decay, pre-delay, damping, width, mod, ducking, HP/LP, shimmer amount, **FREEZE** |
| **Output** | Volume | Auto Gain (level-matched to the input), width, global mix, safety limiter + clipper. | Ceiling, clip character, oversampling (real-time / render) |

### SFX types

| Type | P1 | P2 | P3 | P4 |
|---|---|---|---|---|
| Widener (mono-safe) | — | Side | Low keep | — |
| Auto Double | Drift | Delay | Spread | — |
| Chorus Vintage / Modern | Rate | Depth | — | — |
| Flanger | Rate | — | Manual | Feedback |
| Phaser | Rate | — | Stages (4/8/12) | Feedback |
| Tremolo | Rate | Stereo phase | Shape | — |
| Auto-pan | Rate | — | Shape | — |
| Telephone / Radio | Phone↔Radio | Drive | Noise | — |
| Megaphone | Tone | Drive | Noise | — |
| Lo-fi | Bits | Rate | Noise | Wow |
| Tape Wobble | Wow | Flutter | Saturate | HF loss |
| Ring Mod | Freq | LFO | — | — |
| Auto-wah | Sens / Rate | Range | Resonance | Env↔LFO |
| Octave Down / Up | Grain | Tone / Low cut | — | — |
| Harmonizer | Voice 1 (st) | Voice 2 (st) | Spread | Detune |
| Breath Layer | Tone | Amount | — | — |
| Air Layer | Freq | Drive | — | — |
| Stutter | Gate↔Repeat | Duty | Smooth | — |
| Robot | Note | Buzz | — | — |
| Vocoder | Root note | Chord | Noise | — |

Rate-based effects can sync to the host tempo (**SYNC** + division). The pitch effects (Octave, Harmonizer) follow the detected pitch of your voice. This keeps them clean on sustained notes. They are quieter on consonants and breaths by design.

---

## Presets

- **Factory sections:** Default, Lead, Rap / Hip-hop, Pop, Rock, R&B / Soul, Backing / Stacks, Podcast / Spoken, FX.
- **User presets:** **Save** writes them to `Documents\Vocal Studio\Presets\<section>\` and they appear in the list under **USER / <section>**. Presets saved under the old VocalForge name are copied over automatically.
- Presets never change **Sensitivity**, oversampling, or any **locked** knob.

## Latency and CPU

- Latency is fixed while you work: a 5 ms look-ahead plus the oversampling filters (about 5–5.3 ms at 48 kHz). It changes only when you change the oversampling setting.
- CPU with everything switched on is about 3 % of one core at 48 kHz (2× oversampling).
- The Render oversampling setting is used when the host renders offline.

## Not included in this version

Formant shifting, a key/scale-aware harmonizer and a spring reverb are planned for a later version. The Harmonizer currently uses fixed intervals.
