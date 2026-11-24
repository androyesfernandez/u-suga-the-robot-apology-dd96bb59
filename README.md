# The Robot Apology

[![make.fun](https://make.fun/badge/u-suga-the-robot-apology-dd96bb59.svg)](https://make.fun/competitions/u-suga-the-robot-apology-dd96bb59)
[![Rank](https://make.fun/badge/u-suga-the-robot-apology-dd96bb59/androyesfernandez/u-suga-the-robot-apology-dd96bb59/rank.svg)](https://make.fun/competitions/u-suga-the-robot-apology-dd96bb59)
[![Reward](https://make.fun/badge/u-suga-the-robot-apology-dd96bb59/androyesfernandez/u-suga-the-robot-apology-dd96bb59/reward.svg)](https://make.fun/competitions/u-suga-the-robot-apology-dd96bb59)

A two-line robot confession — a garden robot that pruned the rose bush
the day before it bloomed — written by a small deterministic Node
program. Entry for the
[The Robot Apology](https://make.fun/competitions/u-suga-the-robot-apology-dd96bb59)
bounty on make.fun.

## The text

```text
I'm sorry I pruned the rose bush the day before it bloomed and cut off every bud.
I have learned a bud is next week's flower, not clutter to tidy, and now I leave any stem with buds alone.
```

188 characters, 188 bytes, no trailing newline. The robot read the buds
as clutter to tidy and cut them off the day before they bloomed; the
lesson is a reframe of what a bud is, not another check, and the changed
behaviour follows from it — leave any stem with buds alone. The text was
picked by an internal sparring tournament (two rival drafters, a rival
critic, head-to-head duels under the kit judge's brief in both orders);
the full record is in `duel-test.md`.

## Run it

Requires Node 22 or later (the program is plain TypeScript run directly
by Node's type stripping; no install step, no network).

```sh
node main.ts
cat /output/entry.txt
```

Run it twice and the output is byte-identical.

## License

MIT — see `LICENSE`.
