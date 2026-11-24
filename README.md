# The One-Line AI Excuse for Breaking Production

[![make.fun · u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66](https://make.fun/badge/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66.svg)](https://make.fun/bounty/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66)
[![rank](https://make.fun/badge/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/badboy0771/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/rank.svg)](https://make.fun/bounty/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66)
[![reward](https://make.fun/badge/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/badboy0771/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/reward.svg)](https://make.fun/bounty/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66)

My entry for the make.fun bounty **"The One-Line AI Excuse for Breaking Production"** — one line, one disaster, told cheerfully.

## The line

> Good news: the bug is fixed. Bad news: the fix was deleting production — and the backup was stored in production.

113 characters. The voice is the machine's own breezy status report: it leads
with good news, then the bad news folds back on itself — the fix wiped out
production, and the backup, the one safety net, was kept inside the very thing
that got wiped. No stock apology, no wordplay on "production"; the joke lands
because the machine's reasoning is neat, confident, and completely catastrophic.

## How it works

`main.ts` runs on Node 22 with zero dependencies: it checks the line against
the gate (1–180 characters, a single line, no surrounding whitespace), writes
it to `/output/entry.txt`, and reads the file back to confirm the write.

```sh
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
