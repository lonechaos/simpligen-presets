**New pack: Iris-3B (two cards)**
Iris-3B is a new small image model from Speridlabs that paints the picture directly in pixels, with no VAE in between. It is in the Store now as a community pack with two cards.

**Iris-3B**: the base model. 50 steps at CFG 3, about 35 seconds a picture on a 12 GB card. There is a Steps slider (30 to 100; 100 is the model's own reference setting) and a CFG slider.

**Iris-3B Turbo**: Speridlabs' own 4-step version, about 10 seconds a picture. No sliders, and the negative prompt is not used. For the same seed its layout stays close to the base card, so it is a quick way to try prompts before a full render.

What we saw in a first look (3 prompts, 3 seeds each, at 1024x1024):
- **Photographic and coherent**, with fine skin and fabric detail on the base card.
- **Lettering is hit and miss.** A three-word sign came out right on 2 of 3 seeds on both cards.
- **It is a small model.** In a wide shot of a four-piece band, the base card hid the drummer behind the singer on 2 of 3 seeds. Turbo showed all four on 3 of 3.
- **Turbo is smoother.** Freckles we asked for came out much fainter on Turbo than on the base card.
- **Small faces smear** in wide shots, as they do on most models at this size.

Good to know:
- Stay near 1 megapixel. The sizes in the picker are the ones each card is meant for.
- Both cards use the Qwen3-VL 4B text encoder that the Krea 2 cards use. If you have a Krea 2 card installed, the base card downloads only 3.4 GB; Turbo is 6 GB.
- The base card's file is INT8 and needs an RTX 20-series card or newer.
- The app installs one extension for it (ComfyUI-Iris by Nynxz). Needs SimpliGen engine 0.38.0 or newer.
- Leave the negative prompt empty on the base card unless you need it.
- Prompts are plain descriptive English.

Not in the pack: Iris's upscaler and depth models, and image editing (no edit model has been released yet).

Licence: Apache-2.0. Model by Speridlabs (speridlabs/iris-3b on Hugging Face). ComfyUI support and the INT8 file by Nynxz.
