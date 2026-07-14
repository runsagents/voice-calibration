# voice-calibration

Every AI draft "in your voice" sounds like LinkedIn. This is the method that fixed mine, my agent now drafts messages my friends can't flag, down to the punctuation quirks.

## The method (one afternoon)

1. **Export your own message corpus.** The bigger and rawer the better, chat exports beat polished writing, because your real voice lives in the unedited stuff. Mine was ten years of Telegram, 43,252 messages.
2. **Have the agent study patterns, not content.** Which languages you mix and when, how greetings change per person, message length rhythms, punctuation habits, how you soften requests, how you say thanks, what your era-shifts look like (your 2016 voice is history, not identity).
3. **Make it write a style guide about you, then correct it.** The guide has four parts: a **keep-list** (quirks that ARE you: keep them even if "wrong"), a **fix-list** (typos and autocorrect damage to silently clean), **anti-patterns** (things you'd never say, corporate filler dies here), and **calibrated exemplars** (a few full messages, approved by you).
4. **Blind-test until it passes.** The agent drafts, you judge samples against your real messages, corrections go back into the guide. Stop when you hesitate before spotting your own.

## The template

Copy [`TEMPLATE_SKILL.md`](TEMPLATE_SKILL.md) into your agent's skills as `write-as-<you>`, fill it via the method above, and from then on "draft this in my voice" actually means something.

## Privacy notes

The corpus never needs to leave your machine, point a local agent at it. The finished guide contains *patterns*, not messages, but it's still a fingerprint of you: treat the guide itself as personal data, and don't publish it.

License: CC0 · v1.0.0

,  [@runsagents](https://x.com/runsagents)

## Terminology & prior art
This pattern is known in the field as [authorship style transfer](https://aclanthology.org/2024.findings-emnlp.781/), related to [persona-based generation](https://aclanthology.org/P16-1094/).
This implementation derives the target voice from a personal corpus and calibrates agent output to it.
