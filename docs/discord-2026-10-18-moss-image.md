**New pack: MOSS-Image - text that comes out spelled right (beta engine for now)**
OpenMOSS's MOSS-Image is in the store, two cards: **MOSS-Image** (25 steps) and **MOSS-Image Fast** (8 steps with lodestones' speed LoRA). Its strength is lettering: posters, signs, menus and handwriting come out spelled right, Chinese and Japanese included.

To get it: **Settings > Updates > beta**, take the engine update, and the pack installs. On the stable engine the Store shows it as needing the beta engine; it opens on stable by itself once a tagged engine release carries MOSS.

Measured on a 12 GB RTX 4070 Ti:
- **MOSS-Image:** about 20 s per picture when the prompt changes, about 14 s for another seed of the same prompt.
- **MOSS-Image Fast:** about 10 s when the prompt changes, about 3 s for another seed.
- Output matched plain ComfyUI pixel for pixel, in the app and on the bare engine.
- A handwritten Japanese menu and a Chinese sticky note came out character for character.

We also ran six poster prompts through five models: Nano Banana and GPT Image in the cloud, MOSS-Image, Ming and Ideogram 4 locally. Every model got the quoted headlines right, the cloud models were better at dense small print, and MOSS-Image followed layout and style directions most reliably of the three local ones. The video is attached.

Good to know:
- **Put every word you want on the picture in quotes**, and say where it goes. Text you only describe comes out as pseudo-letters.
- Wide 16:9 pictures of one person sometimes drew the person twice. Square, 3:4 and 3:2 are safer for people.
- The Fast card gives smoother, retouched-looking skin and less variety between seeds. Use the 25-step card for portraits.
- One 14 GB download covers both cards.

Thanks to OpenMOSS for the model (https://huggingface.co/OpenMOSS-Team/MOSS-Image-SFT), Comfy-Org for the int8 files, and lodestones for the 8-step LoRA (https://huggingface.co/lodestones/MOSS-Image-SFT-8-steps-dmd). Apache-2.0.
