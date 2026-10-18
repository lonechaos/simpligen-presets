**Six posters, five image models: what actually gets the text right?**
We ran the same six poster prompts through two cloud models and three that run locally in SimpliGen, and put the results side by side in the video below (1:51, narrated).

- **Cloud:** Nano Banana (Google), GPT Image (OpenAI)
- **Local, in SimpliGen:** MOSS-Image, Ming Image Design, Ideogram 4 Instant

The posters: a Y2K collage with a Chinese headline, a two-ink Brooklyn screenprint, a smartphone ad with four feature cards, a 1970s funk poster, an "Animate with AI" mixed-media poster, and a "STAY CUTE!" typography clipping mask.

What we found:
- **Every model got the quoted headlines right**, including the Chinese one.
- **The cloud models lead on small text.** GPT Image even fills the margins with fine print you can read, where the local models make pseudo-text.
- **MOSS-Image was the most reliable local model** on layout and style directions: the screenprint stayed two inks, and all four feature-card headings came out right.
- **Ming had the most authentic illustrated look** (the 1970s poster). **Ideogram made the most text mistakes:** "GALLERRY", a doubled headline, a made-up web address.
- **Nobody got the clipping mask clean.** GPT Image and Ming put the photo between the letters instead of inside them.

The biggest lesson came before any of that. Our first round used prompts copied straight from PromptHero, written for other models, with Midjourney flags, pasted negative lists and references to images we never supplied, and they went badly. Rewritten for these models, the same posters came out right. The rule: **put every word you want on the poster in quotes**, and say where it goes. Text you only describe comes out as pseudo-letters.

How we ran it: the local models had three seeds each and the video shows seed 11. The cloud models had one image each. Judging is ours, from the images.

MOSS-Image is in the store now as a community pack (beta engine for now). Ming Image Design and Ideogram 4 were already there.
