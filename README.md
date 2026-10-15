# Coverage

**A live-switching drill for learning to cut on the beat.**

Coverage puts a student in a director's booth. A short, scripted pixel-art scene plays out while six cameras cover it at once. The student cuts between them live, one tap per cut, with no undo. When the scene ends, the edit is scored against a reference cut, both for showing the right thing and for cutting at the right moment.

It is one self-contained HTML file. Nothing needs to be installed or run, and it works in any current desktop or tablet browser.

Built by Steve Marsden (Stephen F. Austin State University) with Claude, for teaching introductory film editing.

---

## Running it

Open `index.html` in a browser. To host it, place the file on any static web host, or turn on GitHub Pages for this repository (Settings → Pages → deploy from the `main` branch).

The page loads three typefaces from Google Fonts. Without a network connection it still works and falls back to system fonts.

## The scene: *The Last Booth*

A diner after midnight, in the rain. Ida, the waitress, serves the one customer left, a stranger in a hat. He slides a photograph across the table. The lights die. When Ida turns to the window, a girl is standing in the rain with her hands flat on the glass. The scene runs 48 seconds.

### The six cameras

| Key | Camera | What it's for |
|---|---|---|
| 1 | Wide | The room: geography, and events that affect everyone |
| 2 | CU Ida | Her lines and, more importantly, her reactions |
| 3 | CU Stranger | His lines |
| 4 | Over her shoulder | Him speaking, with her still in the frame |
| 5 | Insert: table | Objects and hands: the pour, the photograph |
| 6 | Window (her POV) | What she sees when she turns |

## How a take works

1. **Choose a starting camera.** Tap it, or press its number key.
2. **Roll the take.** Press **Roll take** (or the space bar). A 3-2-1 countdown with slate pips follows, and then the take is live.
3. **Cut.** Tap a camera tile or press **1–6** to put it on air. The program monitor shows a red tally, burned-in subtitles, and timecode.
4. **Review.** When the scene ends, the **Your cut** panel opens with the score, a timeline, and a beat-by-beat table.

### Practice supports

- **Cue hints.** An amber meter counts down to each beat, and the camera the beat wants is outlined. With hints off, the beat sheet also hides the wanted shots, so students cut from the script alone.
- **Speed.** Students can run the scene at 1×, ¾×, or ½×.
- **Sound.** Students can turn the audio track off.
- **Best score.** The best take is remembered in that browser.

## The beat sheet

The script is broken into 14 beats. Each beat has an ideal cut point, a preferred camera, any acceptable alternate cameras, and a one-line reason a student can argue with:

> **06 · The photograph** (13.9s): *The scene turns on this object. Only the insert shows it.*
>
> **07 · Her reaction** (18.3s): *Let us read her face before she speaks. Hold it.*
>
> **12 · The window** (37.3s): *Her look motivates the cut. Give us her point of view.*

The beats are written so that the right angle follows from what the moment is about. That covers the speaker and the listener, a decisive object, an event that affects the whole room, and an eyeline that motivates a point-of-view cut.

## Scoring

Each beat is worth 5 points, for a total of 70.

- **Angle (2 points).** 2 points for the preferred camera, 1 for an acceptable alternate, and 0 otherwise.
- **Timing (3 points).** Points depend on how close the cut lands to the beat:

  | Distance from the beat | Points |
  |---|---|
  | Within ±0.25s | 3 |
  | Within ±0.5s | 2 |
  | Within ±1s | 1 |
  | Further than 1s | 0 |

  A beat that the right shot simply holds over, without a new cut, earns 1 point.
- **J-cuts.** Three beats accept a J-cut, where the next line starts over the previous shot and the picture cut follows partway into it. A J-cut in those windows gets full timing credit instead of being marked late. J-cuts count only when sound is on.
- **Flash cuts.** Any shot shorter than half a second costs a point.

The total maps to the editor's ladder: **Assembly → Rough Cut → Fine Cut → Picture Lock.**

The review panel shows:

- the student's cut on a timeline against the dialogue and the reference cut;
- the offset of every cut in seconds;
- a single tendency note, such as *"You tend to cut late, by about 0.31s,"* with the reason editors usually cut slightly ahead of a line.

Tapping any row replays the student's cut from two seconds before that beat. **Play reference cut** shows the model edit.

## Sound

All the sound is synthesized in the browser, so there are no audio files:

- **Room tone:** rain on the glass, the refrigerator hum, and the buzz of the neon sign.
- **Foley:** the pour rises in pitch as the cup fills. The photograph scrapes across the formica. Hands knock on the window glass.
- **The blackout:** the lights pop and die, and the hum and buzz drop out with them, so the silence becomes the cue.
- **Score:** a low, beating drone sits under the window reveal.
- **Voices:** syllable-timed babble, pitched for each character, rather than real speech. Ida's question rises at the end.

Under the monitor, a **sound lane** scrolls like an editor's timeline. It shows the student's picture cuts as they are made, his and her dialogue as colored blocks, and the sound effects. Students can see a line coming before they hear it.

## Layout: docked or floating

**Floating** is the recommended mode, and it is the default on any screen 900 pixels wide or more. Every part of the booth becomes its own window on a single screen:

> Program · Cameras · Sound lane · Cue · Transport · Beat sheet · Your cut

- **Move** a window by dragging its title bar.
- **Resize** it with the grip in the bottom-right corner.
- **Snapping:** window edges snap to the screen edges and to each other.
- **Collapse** a window with the **–** button, or by double-clicking its title bar.
- **After a take**, the review window comes forward on its own.
- **Saving:** the layout is saved in that browser. **Reset layout** restores the default.
- **Full screen** hides the browser's own toolbars where the browser allows it.

**Docked** mode, under **Dock panels**, stacks everything as a single scrolling page. That suits narrow screens.

The panels cannot detach into separate browser windows. To spread the booth across two monitors, stretch the browser window across both and arrange the panels inside it.

## Why it works this way

### What it trains

Coverage isolates one skill: feeling where a cut belongs, and committing to it. Walter Murch, in *In the Blink of an Eye*, ranks what a cut should serve, in order: emotion, story, rhythm, then eye-trace and spatial continuity. Every beat here asks the student to judge the first three. What is this moment about? Whose face carries it? When does the thought complete?

### Why live, with no undo

A nonlinear editor lets students scrub, try every option, and undo freely, and deliberation can stand in for instinct. Live switching takes undo away. The student either makes the cut as the moment arrives or misses it, as a multicam television director does. The review then brings the deliberation back, after the student has committed. The student acts on instinct first and examines that instinct afterward.

### Why these six angles

Master, two singles, an over-the-shoulder, an insert, and a point of view make up standard dialogue coverage. Students learn that each angle has a job:

- **The insert** is the only shot that can show the photograph.
- **The reaction beat** (07) cuts to the listener rather than the speaker. This corrects the most common beginner habit, cutting back and forth to whoever is talking.
- **The wide** is the shot when something happens to the whole room.
- **The point-of-view cut** is motivated by Ida's look. It is the Kuleshov principle, learned by doing before it is named.

### Why pixel art

Pixel art is cheap to produce, free of rights problems, and legible at thumbnail size, which matters with six live feeds on a tablet. It also means the faces are crude, so performance can't carry the scene. Whatever meaning the scene has comes from which shot is on screen and when, and that is the lesson.

### Why score it

The scoring follows what research on deliberate practice describes: a narrow target, immediate and specific feedback, and fast repetition. Splitting the score into angle and timing tells students whether they missed **what** to show or **when** to show it, which are different failures. The tendency note turns scattered misses into one habit they can correct. The grade names come from the stages of real editing, so a low score reads as an early draft rather than a failure.

## Known limits

- **The reference cut is one reading, not the truth.** A strong editor could argue for staying on the stranger through Ida's reaction, to withhold her face. The tool rewards one defensible cut.
- **It teaches classical continuity grammar.** Eisenstein's collision montage, Godard's jump cuts, and Resnais's associative cuts would all score badly. That is defensible for an introductory course, but it should be said out loud in class.
- **J-cuts only.** Sound pre-lap (the J-cut) is supported. Letting a line run over the next picture (the L-cut) is not yet scored.
- **One scene.** Students can memorize it, so later takes are partly recall.

## Suggested classroom sequence

1. **First take:** at ½× with hints and sound on. Compare it against the reference cut.
2. **Second take:** at full speed with hints off. Students note their tendency line.
3. **Break the reference:** students make a cut that scores poorly but that they can defend in 250 words, for example by withholding the photograph or never showing the window. This makes them argue with the scoring.
4. **Transfer:** students mark the beats of a real two-person dialogue scene from the screening list, then check where the film's editor actually cut.

## Technical notes

- Everything is in a single `index.html`: inline CSS and JavaScript, with no frameworks or build step.
- The pictures are drawn rectangle by rectangle on 160×90 canvases and scaled up with crisp pixel edges.
- The sound uses the Web Audio API: oscillators, filtered noise, and envelopes. Browsers only allow sound to start after the user interacts with the page, so it begins when the user rolls a take or presses a camera.
- The layout and best score are kept in `localStorage`. The page works the same without it.
- The scene's data is held in arrays near the top of the script, so a new scene means writing new drawing functions and new beat and line tables:
  - `BEATS`: the cut points, wanted cameras, acceptable alternates, J-cut windows, and reasons;
  - `LINES`: the dialogue and action, with timings;
  - `FX`: the sound effects.

## License

MIT. See [LICENSE](LICENSE).
