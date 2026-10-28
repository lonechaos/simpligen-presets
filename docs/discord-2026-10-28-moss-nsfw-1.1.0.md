**MOSS-Image NSFW Finetunes 1.1.0: two more cards, Jib Mix Moss Realistic and Prime Lust Moss**
The pack now has four NSFW MOSS-Image finetunes, two fast and two slower. Like everything MOSS, it needs the **beta engine** for now (Settings > Updates > beta). Each new card is a 5 GB download if you already have the MOSS-Image pack, which supplies the text encoder and VAE.

**Jib Mix Moss Realistic** (J1B, V2): the fastest card in the pack, 12 steps at CFG 1, about 13 s on a 12 GB card. The speed LoRA is built in. It has a natural amateur-photo look, with real-looking skin and lived-in rooms rather than a retouched studio. In our test it drew the sharpest anatomy of the four.

**Prime Lust Moss** (CrHasher, v1.0 max-nsfw): 25 steps at CFG 3.5, about 37 s. The most explicit of the four, with a glossy, tanned glamour look. Its sex scenes were the easiest to read.

How we picked them: six NSFW prompts on two seeds each, against the PornMaster and Artius cards already in the pack, then a round of hand-written prompts in the app. All four cards give interesting and quite different takes on the same prompt, so it is worth trying a prompt on more than one.

Good to know:
- **Write sentences, not Pony-style tag lists.** MOSS was trained on descriptions. A prompt of `masterpiece, best quality, 1girl, 1boy...` with a LoRA trigger word went badly on all four cards (and on the Pony LoRA it was written for). Rewritten as plain sentences, it worked.
- **Say who does what to whom, early.** On a spanking prompt where the action came last, all four cards swapped the roles. Put the action and the position in the first sentence.
- **Jib Mix can draw a different sex position than you asked for.** On missionary it drew the couple sitting face to face on both seeds. Naming the position first helps.
- **Prime Lust: check close-up anatomy on complex positions.** One of its missionary pictures put things in the wrong place.
- **Say "woman" and "man" with an age.** On MOSS, "girl" and "boy" draw young-looking people.
- Two finetunes we wanted are not in the pack because they are paywalled on Civitai: PornMaster Moss V2 (paid download, permanently) and 0x7 Realistic Freedom "Resilience" (Early Access until November 7, so we will look again after that).

Licence flags on Civitai for both new cards: Image, RentCivit, Rent.

Thanks to J1B for Jib Mix Moss Realistic (https://civitai.com/models/3016339), CrHasher for Prime Lust (https://civitai.com/models/2793689), and OpenMOSS and Comfy-Org for MOSS-Image and the native ComfyUI support every card runs on.
