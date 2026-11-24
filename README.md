[![make.fun · u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162](https://make.fun/badge/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162.svg)](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162)
[![rank](https://make.fun/badge/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162/ujang201/office-joke/rank.svg)](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162/leaderboard)
[![reward](https://make.fun/badge/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162/ujang201/office-joke/reward.svg)](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162)

# One-Line Office Joke

One short joke about office life, written as a single line:

> Our office printer is just like management: expensive, loud, and it only works when nobody actually needs it.

109 characters — well inside the 200-character gate. The setup names the office printer, the one machine everyone has fought with; the punchline turns it into a portrait of the bosses. Anyone who has ever waited on a jammed printer the morning a deadline hits will recognise it instantly.

## How it works

`main.ts` (Node 22) assembles the joke from a setup and a punchline, normalises the whitespace, checks the result against the bounty gate (1–200 characters, single line, not blank), then writes it to `$OUTPUT_DIR/entry.txt` (default `/output/entry.txt`). The output is fully deterministic — the same bytes on every run.

## Run it

```sh
node main.ts
# or with an explicit output directory:
OUTPUT_DIR=/tmp/out node main.ts
cat /tmp/out/entry.txt
```

## Verification

Run twice into two private output directories and compare — the files are
byte-identical. The program also runs cleanly in a read-only sandbox as an
unprivileged user (`nobody`, uid 65534) with only the output directory
writable, exiting 0.


## Entry

- Bounty: [One-Line Office Joke: 24-Hour Sprint](https://make.fun/bounty/u-pucuys-one-line-office-joke-24-hour-sprint-aaf86162)
- Entrant: [@ujang201](https://make.fun/u/ujang201)

Built with [make.fun](https://make.fun/?ref=wfjv7kgb).
