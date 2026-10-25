**New pack: MiniMax H3 (Singularity v2) - the Singularity look, now with motion**
WarmBloodAban released a pruned version of Singularity v2 on 23 October, the same 21 GB size as the v1.3 file the Singularity pack uses, so it fits the same machines. One checkpoint, three cards: **Text to Video**, **Image to Video**, **Reference to Video**.

Measured against the v1.3 pack (12 GB RTX 4070 Ti, 5 s at 480p, 20 steps, text to video, three prompts and three seeds, same seeds on both):
- **More motion, on every seed:** 38% more on a tracking cyclist shot, as much as H3 Midnight, and 22% more in a sword duel, more than Midnight. It was the only model whose duellists actually crossed blades.
- **Darker still, on every seed:** a dim studio portrait came out at half v1.3's brightness, and a sunlit courtyard at about two thirds.
- **Tighter framing** on every prompt.
- Close-up faces are as crisp as v1.3's.
- Same speed as v1.3. Through the app with Faster Attention on, all three cards took about 2 minutes per 5 s shot at 480p.

Good to know:
- v1.3 stays as it is. Pick v1.3 for the calmer look, v2 when the shot has to move.
- The numbers above are from Text to Video. Image to Video and Reference to Video were checked in the app on three seeds each: every Image to Video clip started on the picture (and ended on the last-frame picture when one was given), and Reference to Video kept the face on every seed. A two-person reference shot kept both people and spoke its line word for word.
- The author says v2 also fixes audio references and follows the style you name in the prompt better (photorealistic, cinematic CG, 3D CG). We did not measure either.
- v2 is its own 21 GB download from Hugging Face. The model card says Apache-2.0, but it is built on MiniMax H3, so the H3 Community License applies.

Thanks to WarmBloodAban for the model: https://huggingface.co/WarmBloodAban/Minimax-h3_Singularity
