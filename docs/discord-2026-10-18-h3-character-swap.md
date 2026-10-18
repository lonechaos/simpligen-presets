**New pack: MiniMax H3 (Character Swap) - swap one person, keep everyone else**
akatz-ai's Character Swap LoRA for MiniMax H3 is in the store, one card. Give it a clip and a picture of your character, and say who to replace. The camera, the background, the motion and everyone else in the shot stay as they are, and the clip keeps its own soundtrack.

How to use it:
- **Reference Video 1:** the clip. **Character:** a picture of your character (a full-body front view or a character sheet works).
- **Prompt:** only who to replace, for example "the woman in the red coat on the right" or "the man on the left". The card writes the rest of the instruction.

Measured on a 12 GB RTX 4070 Ti, 5.2 s at 480p:
- About 5 minutes per clip (311-316 s through the app).
- On a two-person café shot, only the chosen woman changed, on 3 of 3 seeds. The man next to her stayed the same.
- Across four clips and three seeds each, the swap held 12 of 12 times. The mouth follows the original performance frame for frame.

How it compares with Viggle Animate:
- **Pick this one** when you need one person changed in a group shot. It also has no non-commercial part: no Flux repaint step.
- **Pick Viggle** for a single person when the face should match your character sheet as closely as possible. It is also about twice as fast.

Good to know:
- The new face is a blend: it keeps some of the original performer's brows, face shape and smile. Close, not exact.
- Small accessories can get dropped. A backpack from our character sheet showed up on some clips and not others.
- It uses the official MiniMax H3 base, encoder and VAEs, so if you already have an H3 pack, the new download is 2.1 GB.
- We only tested 5.2 s at 480p. Longer clips, 768p and two look-alike people are untested.

Thanks to akatz-ai for the LoRA (https://huggingface.co/akatz-ai/MiniMax-H3-Character-Swap-LoRA) and lightx2v for the Turbo LoRA. MiniMax H3 Community License + Apache-2.0.
