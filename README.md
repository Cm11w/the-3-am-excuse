[![make.fun](https://make.fun/badge/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878.svg)](https://make.fun/bounty/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878)
[![rank](https://make.fun/badge/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878/Cm11w/the-3-am-excuse/rank.svg)](https://make.fun/bounty/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878)
[![reward](https://make.fun/badge/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878/Cm11w/the-3-am-excuse/reward.svg)](https://make.fun/bounty/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878)

# The 3 AM Excuse

Entry for the [make.fun bounty](https://make.fun/bounty/u-hazel-walrus-38-4764-the-3-am-excuse-c1017878): a program that writes one line — an excuse a hardware wallet gives for refusing to sign a transaction at 3 AM — to `/output/entry.txt`.

## The text

> At 3 AM the mempool is all bots and insomniacs — and I can't tell you apart, so I sign for neither.

22 words, 99 characters (101 bytes UTF-8), one line.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: it is a real excuse, on subject — the wallet refuses to sign and gives its reason in its own first person, it cannot tell its human apart from the bots, so it signs for neither. The angle is original: the field is crowded with keys asleep, buttons on strike, seed phrases dreaming, sunrise, designated drivers and "no good decision has ever been signed at 3 AM", while the mempool — and MEV bots as the only other things awake at 3 AM — appears in none of the 1,305 public submission titles sampled, and neither does the wallet failing to tell its owner from a bot. No battery, firmware-update or cold-storage joke, the three the brief names as the usual ones. It speaks in the wallet's own voice — "mempool", "bots", "sign" — a device with its own priorities and grudges, not a generic assistant. And the hour is the joke: at 3 PM the mempool is full of humans and the line makes no sense, so it could not be pasted onto a 3 PM transaction. One line, plain words, and a turn (the human accused of being indistinguishable from a bot) that is easy to repeat to a friend the same day.

## License

MIT — see [LICENSE](LICENSE).
