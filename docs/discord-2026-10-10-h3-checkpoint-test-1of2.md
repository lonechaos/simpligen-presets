**MiniMax H3: eight checkpoints, one scene, three ways of writing the prompt**
We took DeCat's "Last Snow Globe" scene (a felt stop-motion man sweeping church steps, his world tilts, a giant eye appears in the sky and blinks) and ran it on eight H3 checkpoints with the same seed: 15 seconds, 480p, each card at its own default steps. 24 renders, all on a 12 GB card.

**The big result is about prompts, not checkpoints**
- **Plain prose:** every checkpoint gave one continuous shot, and every one ran late (the tilt at 8 s instead of 5, the eye at 11-12 s instead of 10).
- **A structured brief with three timed shots:** every checkpoint gave three shots with clean cuts at 5 s and 10 s, and a single eye.
- **An automatic rewriter (lightx2v's):** in between. It got the big eye on four checkpoints, a small one on three, and two eyes on one.
