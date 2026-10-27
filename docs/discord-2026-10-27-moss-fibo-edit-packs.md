**Two new image-edit packs: MOSS-Image Edit and Fibo 2.0 Edit**
Both do the same job - hand them a picture and a sentence naming the change and what to keep - and both need ComfyUI 0.43.0, so for now they are **beta engine only** (Settings > Updates > beta, app 1.76.2 and up). Stable is still on 0.42.0 and will not see them until it is promoted.

**MOSS-Image Edit** - one card, on the same weights the MOSS-Image pack already downloads, so it is only a **283 MB** extra if you have that pack. 30 steps, CFG 1, about 15 s on a 12 GB card. Colour, outfit, lighting, season and visual style all work, and **lettering in the picture survives letter-exact** - a shop front with two painted signs came through unchanged in all six arms we ran, including a flat-vector restyle and a rainy-evening relight. The thing MOSS is best at is not lost in the edit.

**Fibo 2.0 Edit** - Bria's Fibo 2.0 Edit Turbo, 8 steps, about 14 s, 13.3 GB download. Of the two it is the **stronger editor**.

We ran them head to head on the same pictures, instructions and seeds - 3 sources x 3 kinds of instruction x 2 seeds, 18 arms each:
- **Fibo recolours an object where MOSS redraws it.** Told to turn a red bicycle yellow, Fibo returned the same bicycle - same frame, same fenders - while MOSS changed the frame shape on one seed and added a wicker basket nobody asked for on the other.
- **Fibo is better at leaving things alone.** "Repaint the shop front, keep both signs" - Fibo kept the chalkboard's frame, MOSS repainted it.
- **Fibo holds faces closer.** On a dress recolour the face moved about half as far from the original; on a golden-hour relight MOSS washed the whole face orange while Fibo kept the warm light on the hair.
- **Lettering is a draw.** Both letter-exact in 12 of 12 arms.
- **MOSS wins a heavy style change.** Photo to watercolour: MOSS keeps the face plainly the same person, Fibo's is more convincingly painted but drifts further.

Good to know:
- **Pick the aspect ratio that matches your picture.** A different ratio centre-crops it first. Fibo holds up fine; the MOSS card gets noticeably looser, lettering included.
- **Say what to keep, not just what to change.** "Change only the red bicycle to yellow. Keep everything else in the street exactly as it is" does far better than the first half alone. Where something still drifts, name it: adding "keep his blue eyes" and "keep the plain grey backdrop" fixed both on the next run.
- **Small objects get redrawn rather than recoloured on the MOSS card**, and a "change only X" instruction can spill onto a neighbouring surface. Fine texture softens a little.
- **Non-Latin text:** two independent tutorials report Fibo returning gibberish for Chinese and failing Hindi, where MOSS renders both. We have not measured this ourselves - if you work in CJK, MOSS is the safer pick.
- **Licences.** MOSS-Image is Apache-2.0; its edit LoRA declares no licence for its weights. **Fibo 2.0 is CC BY-NC 4.0 - non-commercial use only. Selling the pictures, or using them commercially, needs a separate agreement with BRIA AI** (platform.bria.ai/licensing). Worth reading before you build anything on it.

Thanks to chinoll for the MOSS-Image Edit LoRA (https://huggingface.co/chinoll/Moss-Image-Edit), OpenMOSS for MOSS-Image, BRIA AI for Fibo 2.0 (https://huggingface.co/briaai/Fibo-2.0-dev), and Comfy-Org for the repacks and the native ComfyUI support that both cards run on.
