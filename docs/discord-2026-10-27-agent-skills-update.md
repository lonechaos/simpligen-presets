:clapper: **Agent Skills for Media Creation: October update** - what we learned this month, added to all three skills

**minimax-h3-prompt**
- **Singing a real song:** give H3 the song's vocal stem as reference audio, with the lyrics and their times in the brief, and it lip syncs the performer to it (two checkpoints, three seeds each).
- **Voice references:** attach them in the order the characters first speak. H3 ignores the labels and swaps the voices otherwise. Use WAV, not MP3: the compression carries into the voice.
- **Silence:** `overall_soundscape: None.` does not give you silence; name what should be heard instead. `None.` on `non_diegetic_music` does keep the score out.
- **Extra words:** any English in the prompt can end up spoken, including text a workflow adds behind your back.
- **Extra musicians:** a solo close-up grows the rest of the band when the prompt or soundscape mentions other players. Say "alone" and name only that instrument.
- **Drafts:** a 480p draft confirms timing and words, not who lip syncs. Check the mouths again on the final render.

**vrgdg-music-video-builder**
- **Sparks and glassy smoke that survive retakes come from the locked song audio.** Render cutaways with silence and sung scenes with the vocal stem only, then lay the song back over.
- **Lyric timing:** force-align the lyrics you already have instead of transcribing them. It was about ten times more accurate in our test. Times called out by ear run about a second late.
- **More to check:** band members at a mic mouthing the lead vocal, and invented people walking into empty space behind a close-up.

To update, run the install command again:
```
npx skills add michaeldune/agent-skills-for-media-creation
```
Repo: https://github.com/michaeldune/agent-skills-for-media-creation
