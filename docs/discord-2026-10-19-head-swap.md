**New card: MiniMax H3 Head Swap - a new face and hair, the outfit stays**
The **MiniMax H3 (Character Swap)** pack now has a second card, **MiniMax H3 Head Swap** (pack 1.2.0, so update the pack if you have it). It uses UntMods' Face Swap LoRA: give it a clip and a picture of a head, and the person in the clip gets the new face and hair while their clothes, props, pose, the background and the clip's own sound stay as they were. The mouth follows the original performance.

How to use it:
- **Reference Video 1:** the clip. **Head:** a picture of the head, **cropped above the shoulders** (face and hair only). Anything else in the picture comes along: a sweater in the crop ends up on the person.
- **No prompt needed.** Leave it empty.
- A full character sheet does not work here: with one, the face mostly stayed the original's. Use a head crop. For a whole-person swap (face, hair and clothes from a sheet), use the Character Swap card.

Measured on a 12 GB RTX 4070 Ti at 480p:
- About 5 minutes for a 5 s clip, about 8.5 minutes for 7 s.
- With a head that looks clearly different from the performer (a woman of about 65 with a silver bob), the head changed on 12 of 12 clips (4 clips, 3 seeds each), and the clothes, props and background stayed on all 12.

Both cards now take **Duration 5 to 10 s**. Past 8 s the model no longer fits on a 12 GB card and it gets much slower: 10.8 s took 1 h 48 min on ours. On a bigger card that is not an issue.

Good to know:
- **Two people in the shot?** It cannot pick one, and it may change both: on our two-person cafe shot the man changed too on 1 of 3 seeds.
- The hair can keep the original's shape and take only the new colour: wet, slicked-back or very long hair did that.
- Only the head changes, so a 65-year-old face can end up on a 25-year-old's body. The face is a blend and can look younger than your picture.
- If you already have an H3 pack, the new download is 2.0 GB.

The video is attached. Both women's voices are H3's own: the swap keeps the clip's soundtrack, so the first line is still the original performer's voice, and the second clip is the swapped character speaking for herself.

Thanks to UntMods for the Face Swap LoRA (https://huggingface.co/UntMods/FaceSwap_MiniMaxH3_REF2VA) and lightx2v for the Turbo LoRA. Apache-2.0.
