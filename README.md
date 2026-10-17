# HSK Lexicon

**Live site:** https://hsk.quannk.com

A self-study guide to Mandarin for everyday conversation, built on the HSK 3.0 word list, levels 1–5 (4,316 words). It has four parts:

- **Words:** 20 words a day. Each word has tone-coloured pinyin, a recording, its meaning, and three example sentences. Every example has pinyin, audio, an English translation and a short analysis of what the word does in it. Each day ends with a test.
- **Conversations:** model dialogues for everyday situations. Each comes with structure labels, a meaning for every word, and audio for every line. There are also pattern templates, a phrase bank and words grouped by topic.
- **Glossary:** tones, sounds, spelling rules and tone changes, with a pinyin chart and optional listening drills.
- **Progress:** which words you have opened and how your tests went.

It runs entirely in the browser, with no account and no install, and it works on a phone.

---

## Why I built it

I wanted the format that worked for my [GRE Lexicon](https://github.com/quan-nk/gre-lexicon): a fixed set of words each day, examples I can actually understand, and a test at the end. This time it is for Mandarin and for real conversation rather than an exam. Grammar and pronunciation are there when I need them (Glossary), but the daily work is words in sentences and short dialogues.

---

## How to use it

### Every day: Words (about 35–40 minutes)

1. Open **Words**. It opens on the first day you have not finished; use the arrows or the day picker to move between days.
2. Tap each of the 20 word tabs. Every word shows:
   - its pinyin with tone colours and a **speaker button**;
   - its meaning and senses, its measure word, and the Hán-Việt reading of each character;
   - **3 example sentences**. Tap any word in a sentence for its meaning, and tap the speaker to hear the sentence.

   Under **More** you'll find common combinations, related words and dictionary links.
3. **Listen** plays the whole day hands-free: each word twice, then its three examples, then the next word.
4. Finish with the 21st tab, **Test**. It shuffles the day's sentences with the word blanked out.
   - Pick from 4 options, or type the pinyin (tones optional).
   - Missed sentences come back at the end, and the word tabs turn green or red as you go.
   - Switch the pool to "Days 1–N" to review everything so far.

### When a day's words are done: Conversations

Each conversation lists the course day it fits after and how many of its words you have opened. Turn on **Structure** to see what each line is doing (greeting, request, softener, refusal…), and use **Play all** to hear the whole exchange. **Patterns** shows how common exchanges flow, **Phrases** gives several ways to say the same thing, and **Topic words** groups vocabulary by situation.

### When a sound is unclear: Glossary

The tones, initials and finals (with comparisons to Vietnamese sounds), spelling rules, tone sandhi and the neutral tone, plus a pinyin chart where every syllable plays a human recording.

### Handy links

Add these to the address to jump straight to a section:

| Link ending | Opens |
|---|---|
| `#d05` | Day 5 of the words |
| `#d05-test` | Day 5's test |
| `#talk` | The conversations |
| `#c012` | Conversation 12 |
| `#chart` | The pinyin chart |
| `#drills` | Listening drills |

Your progress (words opened, test results, conversations read) is saved in your own browser on that device.

---

## How the content was made, and checked

- **Words:** the HSK 3.0 list (levels 1–5), ordered within each level by how often each word occurs in film subtitles (SUBTLEX-CH), as a stand-in for everyday speech. Meanings start from CC-CEDICT.
- **Examples, analyses and conversations** were written by AI (Claude). A script checks every sentence:
  - every word must be an HSK word at or below the day's level;
  - every pinyin reading must be valid;
  - sentences must stay within a length limit.
- **Levels 1–2** (days 1–64) had two independent AI reviewers per day, one for natural Mandarin and one for the accuracy of every explanation. A fix pass followed. Then a different model re-read every finished file: it found 156 more serious and 883 minor problems, and they were fixed.
- **Levels 3–5** (days 65–217) had a lighter check: one AI draft, then one AI reviewer who also fixed what it found. Expect more slips there.
- **Audio:** words and syllables are human recordings. Sentences and conversation lines use a neural voice (Qwen3-TTS, generated locally). Speech recognition then transcribed each clip back: for levels 1–2, 4,474 of 4,627 sentences and lines matched syllable for syllable.

No native speaker has reviewed the content yet. If you spot a mistake, please open an issue.

---

## Credits and licenses

The guide's content is shared under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), because it builds on CC-CEDICT and on the audio-cmn recordings. See [LICENSE.md](LICENSE.md) for the sources and their notices.

---

## Thank you, Claude

This project would not exist without Claude (Anthropic).
