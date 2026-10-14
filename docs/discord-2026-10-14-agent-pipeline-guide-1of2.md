🎬 **Let an agent run a whole video project (Part 1 of 2)**
An agent connected to SimpliGen can do far more than one render at a time: make the folders, keep your prompts, pick presets, queue every shot, check the results and stitch the film. I made a 56-second short this way. Here is the toolkit and the setup.

1️⃣ **What the agent needs**
- **SimpliGen's MCP server.** See the Antigravity / Gemini CLI guide for connecting it. Claude Code and other MCP agents use the same server.
- **ffmpeg** for trimming, joining, frame grabs and the final mux.
- **WhisperX** to transcribe what each clip actually says.
- **Demucs** to split a song into vocals and backing, for music videos.
- **Python**, which the agent uses to glue these together.

Ask the agent to install whatever is missing and confirm each one runs. On Windows, set `PYTHONIOENCODING=utf-8` before running WhisperX, or it crashes on non-English text.

2️⃣ **One folder per project**
```
my-film/
  refs/       portraits, locations, voice samples
  prompts/    one text file per shot
  renders/    every take, never overwritten
  final/      the edit
  shot-list.md
```
`shot-list.md` is the most useful file you will have. For each shot: the line, the preset, the seed, the prompt file and **which take you picked**. With it, you or the agent can pick the project up days later.

3️⃣ **Your prompt library**
Keep reusable pieces as text files: character descriptions, the location, the voice description, your camera wording. Tell the agent to build each shot's prompt from them, so every shot describes her the same way.

4️⃣ **Choosing presets**
The agent can read every preset's description through `list_capabilities` and choose sensibly. Give it your own rules as well, for example:
- dialogue shots use a lip-sync card
- test at 480p before going higher
- ask before spending cloud credits
