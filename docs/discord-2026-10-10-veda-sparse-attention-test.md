**We tested Veda, the new "sparse attention" speed-up for MiniMax H3**
Veda is a small add-on (275 MB) that works out which 10% of H3's attention actually matters and skips the rest. It is not a LoRA and does not change the model, and it runs on top of Faster Attention. **It is not in SimpliGen.** This is a test report from plain ComfyUI, not a new card.

How we tested: RTX 4070 Ti 12 GB, 8-step turbo models, three seeds each, every clip made with and without Veda (Faster Attention on both times). 38 clips.

**Speed**
- 768p, 5 seconds: about 185-210 s without Veda, 110-130 s with it. That is 1.6-1.7x faster, and it was the same on stock H3, DaSiWa v3 and 10Eros beta5 Turbo.
- 480p, 15 seconds: about 250 s down to 150-165 s. Also 1.6x.
- 480p, 5 seconds: only 10-30% faster.
- Reference to video at 480p: no gain.

**Quality**
- Small faces in a wide shot stayed sharp. This is where the older sparse attention (Sol-Attn) smeared them.
- A scripted spoken line came out word for word, 3 of 3.
- A reference character kept her face and outfit, 3 of 3.
- The catch: on 10Eros beta5 Turbo, a wide shot of a five-piece band lost track of people in 4 of 6 clips. A singer was swapped mid-clip, a drummer vanished, a sixth player appeared. The same shot on stock H3 and DaSiWa v3 was stable in 6 of 6.
- It changes the shot you get from a seed. You get a different clip, not the same clip faster.

**Where that leaves it**
Promising at 768p and for long clips on stock H3 and DaSiWa. Not on 10Eros as it stands. The authors' 2-3x figures are for 10-15 second clips at 768p on 24 GB cards, a size our 12 GB test machine cannot run. Not tested yet: image to video, reference to video at 768p, and inside SimpliGen's engine.
