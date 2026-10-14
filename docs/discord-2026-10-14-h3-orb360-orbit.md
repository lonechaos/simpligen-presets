**New pack: MiniMax H3 ORB360 Orbit (one card)**
Give it one photo and the camera flies a full circle around the subject while everything stays frozen, then lands back on your photo's own view. It is in the Store now as its own community pack, built on MATLOWAI's ORB360 LoRA for H3's reference model.

**MiniMax H3 ORB360 Orbit**: one picture in, a 5-second silent orbit out. About 2 1/4 minutes at 480p and 7 minutes at 768p on a 12 GB card.

What we saw (three photos: a woman full body, a man head and shoulders, a film camera on a table; two seeds each, once at 768p and once at 480p in the app):
- **The camera went all the way round and showed the back of the subject in 5 of 6 clips, both times.** Ponytails, hair ties and the back of the camera body came out sensible.
- **The miss was the full-body woman both times**, a different seed each time: the background kept turning but she turned on the spot. Try another seed if that happens.
- **We tested it against pablodawson's 360 Orbit LoRA** too. That one loops more cleanly and reached the back of people every time, but it spun the camera on the table in place instead of orbiting around it. ORB360 handled both people and objects, so it is the one we packed.

Good to know:
- The prompt box is not used. The card always sends the author's orbit prompt, which is timed to exactly 124 frames, so the length is fixed at 5 seconds.
- We removed one clause from that prompt (about falling snow and dust hanging in the air) because it put frozen white specks on coats, dresses and tables.
- One subject in the middle of the photo works best. Whatever the photo cannot show, the back of the subject and the rest of the room, is invented and can drift: one living room opened onto a lake halfway round.
- The turn is a little uneven, and the last frame is close to your photo but not identical, so a loop has a small jump.
- It uses the H3 reference model, text encoder and VAEs from the official H3 pack. If you have that, this downloads only the 0.6 GB LoRA.

Licence: MiniMax H3 Community License. LoRA by MATLOWAI, on Hugging Face (MATLOWAI/MiniMax-H3-ORB360-CardSpin).
