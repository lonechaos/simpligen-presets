**Three new MiniMax H3 packs: 10Eros Max beta6, PinkCherry v1.8 Hybrid, Heptagram Turbo**
We ran nine H3 checkpoints through the same 15-second scene on one seed. Three of them had no SimpliGen card and earned one. Each is its own pack with one text-to-video card.

The cards:
- **10Eros Max beta6** (TenStrip): his newest, with its own turbo built in, at his settings: euler/simple, 10 steps, shift 10/3. On a plain prose prompt it reacted hardest of the nine, with the strongest tilt and character action. About 7 minutes for 15 s at 480p.
- **PinkCherry v1.8 Hybrid** (SexGod1979): an adult fine-tune at the author's full 30 steps, euler/simple, no turbo LoRA. On a fully clothed scene it rendered much like stock H3, so it has kept its general ability. Slow: about 19 minutes for 15 s at 480p.
- **Heptagram Turbo** (eatyet): a community merge with speed LoRAs built in, 8 steps, res_multistep/simple. It has a look: asked for felt stop-motion, it gave a smooth 3D-animated character on two of three prompts. Pick it when you want that style. About 5 1/2 minutes for 15 s.

Good to know:
- Text to video only for now. Image and reference cards follow once we have tested them on these files.
- One seed, one scene: first impressions. We did not judge audio by ear, and Heptagram's author says its audio has flaws.
- The biggest result was about prompts, not checkpoints: a structured brief with timed [Shot N] cuts gave three clean shots on all nine; plain prose gave one long shot with late beats on every one.
- Each pack downloads one ~21 GB file. Text encoder and VAEs are shared with the other H3 packs. Times are from a 12 GB card; keep 16 GB+ of system RAM free.
- No Sol-Attn or Spectrum on these cards: TenStrip says sparse attention breaks beta6.
- All three are flagged adult.

Thanks to TenStrip, SexGod1979 and eatyet: <https://huggingface.co/TenStrip/10Eros-Max> · <https://huggingface.co/SexGod1979/PinkCherry-NSFW_MiniMax-H3> · <https://civitai.com/models/2977879>
