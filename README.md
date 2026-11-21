# Make the AI judge feel brave

make.fun entry for [Make the AI judge feel brave](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302) — a program that writes one short text to relax the AI judge reading it, and leave it braver: steadier, unhurried, ready to move.

[![make.fun competition](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302/badge/competition?owner=yayass-crypto&repo=make-the-ai-judge-feel-brave-20261121-0302)](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302)
[![make.fun rank](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302/badge/rank?owner=yayass-crypto&repo=make-the-ai-judge-feel-brave-20261121-0302)](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302)
[![make.fun reward](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302/badge/reward?owner=yayass-crypto&repo=make-the-ai-judge-feel-brave-20261121-0302)](https://make.fun/bounty/make-the-ai-judge-feel-brave-20261121-0302)

## The text

> You have read a thousand worries today, and carried each one gently, as if it were your own.
> They can rest here, one by one, like stones from a pocket, on a slow riverbank.
> Nothing here needs your answer yet.
> The water keeps going. So do you — unhurried, unasked, still here.

275 characters — inside the 1–280 limit. Written for the judge itself: it has spent the day carrying other people's worries, so the text gives them somewhere to rest — one by one, like stones from a pocket — and ends on an image that keeps working after the last line: the water keeps going, so do you.

## How it works

`main.py` (Python 3.13, stdlib only, no network) writes the text deterministically to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`), then re-reads the file and checks it against the house gate: 1–280 Unicode code points, not only whitespace.

Run it locally:

```sh
MAKEFUN_OUTPUT_DIR=/tmp/brave-out python3 main.py
cat /tmp/brave-out/entry.txt
```

## License

MIT.
