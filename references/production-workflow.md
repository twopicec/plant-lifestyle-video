# Production Workflow

Read this reference for material review, story planning, subtitles, audio, editing, sound effects, or export work.

## 1. Inspect the source

- Search likely project folders before asking where a file is. Prefer `rg --files`; use `find` only when necessary.
- Read duration, resolution, orientation, frame rate, codecs, sample rate, and channel layout.
- Generate contact sheets or representative stills for visual inspection. Note meaningful cuts and the strongest reveal.
- Listen to or transcribe the final recording. When a supplied script differs from the performance, subtitle what is actually spoken.
- Identify what is absent. Do not add instructions or narration that require missing evidence unless the user wants voice-only context.

## 2. Build the story

Define the one-sentence story before writing the timeline. A useful pattern is:

1. Surprising result or contradiction.
2. Minimal history and the practical trigger.
3. Action with a real pause, resistance, or small failure.
4. Visual reveal and reaction.
5. Two or three useful judgments tied to the footage.
6. Finished home/lifestyle image and a natural closing thought.

For a 60–90 second video, prevent any repetitive action from running more than about three seconds without a new angle, speed change, original sound, or idea. Keep the central reveal at normal speed.

## 3. Voiceover

- Draft for normal conversational speed, then read aloud for breath and emphasis.
- Let emotion follow the story: conversational opening, rising surprise, brief reaction pause, calm useful explanation, warm finish.
- Use sentence-level volume, pacing, and tiny pitch changes only when repairing a flat performance. Preserve identity and avoid obvious voice-changing.
- Re-render emotional versions from the original recording rather than stacking denoise and compression on an already processed file.
- A natural warm repair commonly uses light denoise, a 65–70 Hz high-pass, restrained warmth and clarity EQ, gentle de-essing, and light compression. Treat these as starting points, not fixed presets.
- For a finished spoken track, a practical target is around −16 LUFS with true peak at or below −1.5 dBTP, unless the destination requires otherwise.

## 4. Subtitles

- Align to the final audio; do not stretch or move approved speech timing to match an earlier script.
- Keep phrases short enough for mobile reading and break on meaning rather than arbitrary character counts.
- If the user requests no punctuation, remove all punctuation without changing cue times.
- Preserve every spoken word and sentence ending. Verify the first and last cue against the waveform.
- Deliver a standard subtitle file and, when requested, a readable subtitle review version.

## 5. Picture edit

- Start on action or evidence, not setup.
- Use original handling sounds at tactile beats such as a failed pull, a root ball release, soil movement, or patting a pot.
- Accelerate filling soil and repeated hand movements; keep important texture and the main reveal unhurried.
- Avoid adding a process claim that is not shown. For example, do not say “最后浇透水” when there is no watering footage.
- When only audio is changing, stream-copy the approved video where possible so the picture and subtitle timing remain byte-for-byte stable.

## 6. Music and sound effects

- Use the established library at `/Library/Audio/Apple Loops/Apple/Final Cut Pro Sound Effects/`.
- For a warm home-life bed, audition quiet, unforced tracks and keep music clearly below speech. The creator may choose to add the music personally; honor that split.
- For a coherent playful game palette, use only assets from `星露谷`. Choose effects by story function: whoosh for entry, pickup or selection for a detail, funny fall or cancel for a joke, reward or artifact for the reveal, hoe/dirt for soil, chest or shipment for placement, and success/gift for the finish.
- Layer effects only at the main climax. Elsewhere use one short effect per idea and leave breathing room.
- Make effects audible without masking consonants. Check the mixed track for clipping after codec conversion; true peak should normally remain at or below −1.5 dBFS/dBTP.
- When delivering a separate effects stem, start it at 00:00, match the video sample-exact duration, and use 48 kHz, 24-bit stereo WAV unless another format is requested.

## 7. Exports and review

Use descriptive, non-destructive names such as `检查版`, `无花字`, `无音乐`, `音效合成轨`, or a version suffix. Confirm:

- approved duration, frame count, and dimensions;
- speech completeness and sync;
- subtitle cue count and final cue;
- added music/effects/flower text match the requested inclusion set;
- integrated loudness and true peak are safe;
- the original file and earlier approved versions still exist.

If a planned cue does not match the actual shot, move it to the correct visual moment and report the correction instead of following an inaccurate timestamp blindly.
