🎬 **Let an agent run a whole video project (Part 2 of 2)**

5️⃣ **Render one shot, then look**
Don't let it queue the whole film at once. Have it render one test shot and stop. My first test showed three problems no plan would have predicted: speech starts within a second of the shot beginning, the voice ran slower than expected, and the framing came back wider than asked. Every later shot was better for it.

6️⃣ **Checks the agent can run for you**
- **Words:** WhisperX on every dialogue clip. H3 sometimes adds words after the line; the transcript catches it before you edit. Transcribers often drop the first word, so a missing first word is not proof.
- **Silence:** ffmpeg's `silencedetect` shows where speech ends and whether the hold after it is clean.
- **Pictures:** an ffmpeg contact sheet (one frame per second, tiled) lets the agent check framing, props and continuity without watching every take.
- **Music videos:** Demucs the song first, then check lip sync against the vocal stem, not the full mix.

7️⃣ **Stitching without drift**
Joining clips by gluing their audio together drifts by about 20 ms per clip, and lip sync slides further out with every cut. Have the agent:
1. trim each clip to its exact video length,
2. build the soundtrack as one uncompressed track,
3. mux it with the picture **once**,
4. check each shot's audio against its source clip afterwards.

8️⃣ **What to keep for yourself**
The agent can check words, timing and sync. It cannot hear whether a line is funny, or see whether a face still looks like her. Watch each take and pick it yourself, then have the agent write your choice into `shot-list.md`.

🆘 **If something goes wrong**
- **A job seems stuck:** ask it to check the job and the engine queue before resubmitting. A timeout is not a failure.
- **The machine is slow afterwards:** ask it to unload models when the batch is done.

Questions and results welcome below. 🙌
