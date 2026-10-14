**10Eros Max betas: how long does a 768p clip take?**
A quick speed check of the three 10Eros beta cards on a 12 GB card (RTX 4070 Ti, 32 GB RAM). Text to video, the same prompt and seeds on each, 5 seconds at 768p (1344x768), each card on its default settings. Two runs per card.

- **10Eros beta5 Turbo** (8 steps): about **2 min 50 s**
- **10Eros beta6** (10 steps): about **5 min 40 s**
- **10Eros beta5** (20 steps): about **6 min 10 s**

What's behind the numbers:
- beta5 Turbo is about twice as fast as the other two at this size.
- beta6 has fewer steps than you would guess from its time. Each step takes about 32 seconds, against about 14 on beta5 Turbo. The beta6 card runs with Faster Attention only: its author says the extra step-skipping speed-up breaks it, and that speed-up is what makes the two beta5 cards quick.
- So read this as "how long each card takes as shipped", not as a pure model comparison.

Good to know:
- All six runs finished at 768p on 12 GB. Nothing stalled, but system RAM got down to about 4 GB free, so close other heavy apps first.
- These are 5-second clips. Longer clips at 768p get much heavier on a 12 GB card; drop to 480p or 544p for 10 to 15 seconds.
- Speed only. We did not compare how the clips look in this test.
