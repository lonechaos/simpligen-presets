**New community pack: MiniMax H3 (FastH3 Omni)**

FastVideo and Nuva Lab released FastH3 Omni yesterday: an eight-step MiniMax H3 distill built for references. It takes up to nine pictures, three video clips and three audio files per shot. The pack has one card, Reference to Video.

What I measured on a 12 GB RTX 4070 Ti, same seeds, prompts and references against DaSiWa v4 and Midnight:
- Every identity held and every spoken line came out word for word, on all three.
- The crispest picture of the three, with more of the background in focus.
- About 75 s per five-second 480p shot (DaSiWa v4 44 s, Midnight 97 s).

The audio references are the fun part:
- Drop a voice clip in as an audio reference and the character speaks your new line in that voice.
- Drop a song's isolated vocal in as an audio reference, write the lyrics with their start times in the prompt, and the singer performs that exact vocal, lip-synced.

Needs the v0.42.0 engine. Tested at 480p up to 11.5 s; the higher resolution tiers are there but I have not run them yet. The download is a 22 GB checkpoint plus the usual H3 text encoder and VAEs.
