# Duel tournament — how the winning line was picked

Competition: The Robot Apology (u-suga-the-robot-apology-dd96bb59), $2,
1 paid place, blind rounds, 1,568 submissions at build time. Gate:
1–400 characters. Judge: z-ai/glm-5.3-flash, criteria in order —
(1) is a robot apology, (2) mistake concrete and human-scale,
(3) lesson follows from that exact mistake and names a changed
behaviour, (4) both sentences clean, each doing its own job,
(5) machine voice, warm and a little rueful. No OpenRouter key on
this machine, so all duels below are PROXY judging under the kit
judge's brief verbatim, each pair judged in both orders; a call gives
the picked entry 0.5 + margin/10 (margin 1–5) and the game score is
the mean of the two calls. Bar for submission: mean 0.60+.

## Field scan

Latest 100 of 1,568 submission titles: saturated angles — watering
any plant / plastic plant / laptop instead of fern / drowned cactus;
waking the baby; alarm 7 PM instead of 7 AM; filing/sending the wrong
report to the wrong person; deleting photos / unfinished backup;
vacuuming Lego / hearing aid; ironing a swan / pink shirt; dog's
dinner; oven 220 vs 120; defrosted birthday cake; unplugged fridge.
All drafters were told to avoid these and the brief's own examples.

## Round 1 — two rival drafters, 10 candidates each

Drafter A top 3 (full file in scratch/drafter-a/drafts-a.md):
- A3 dishwasher soap flood, 234 chars, round-robin mean 0.725,
  0.667 vs stock baselines B1/B2/B3.
- A2 shrunk wool sweater, 209 chars, 0.550 / 0.533.
- A4 fork in the microwave, 194 chars, 0.500 / 0.533.

Drafter B top 3 (scratch/drafter-b/drafts-b.md):
- D5 rose prune, 183 chars, round-robin mean 0.65,
  vs baselines 0.65 / 0.50 / 0.40 (mean 0.517).
- D1 dish soap, 212 chars, 0.5875 / 0.533.
- D2 red sock, 194 chars, 0.4875 / 0.433.

Both drafters flagged the same weakness: all six lessons were
procedural checks ("check the bottle/label", "scan for metal",
"look twice"), while the strongest stock baseline (B3, woke baby:
"finished is not urgent, so now I whisper after bedtime") wins
criterion 3 with a conceptual reframe. A reframe lesson was the
upgrade path.

## Round 2 — rival critic

The critic (scratch/critique.md) ranked A3 > D5 > D1 > D2 > A2 > A4,
attacked every S2 as a check with no thought in it, and proposed
revised versions of the top 2 with reframe lessons:

- A3 revised (222 chars): S1 kept; S2 became "I have learned not
  all soap does the same job, and now I only open the tablet drawer
  for that machine."
- D5 revised (188 chars): S1 kept; S2 became "I have learned a bud
  is next week's flower, not clutter to tidy, and now I leave any
  stem with buds alone."
- Untried angle proposed: the recycling — the robot threw away
  handwritten letters (191 chars), plus a tighter variant (203 chars)
  with the behaviour "now I keep every handwritten page until you
  say so". Biggest risk named: a reframe rival on our own angle
  beats an unrevised check-lesson entry on criterion 3.

## Round 3 — coordinator's final cross-duel (6 entries, both orders)

X1 A3 revised (222) · X2 D5 revised (188) · X3 letters (191) ·
X4 letters-tight (203) · X5 A3 original (233) · X6 D5 original (183).

| Entry | Mean game score |
|---|---|
| X2 D5 revised | **0.62** |
| X4 letters-tight | 0.60 |
| X3 letters | 0.56 |
| X1 A3 revised | 0.54 |
| X6 D5 original | 0.36 |
| X5 A3 original | 0.32 |

Key calls: X2 beat X3/X4 0.60 (S1 exactness — "the day before it
bloomed" is the most exact temporal detail in the set), X3/X4 0.70
vs both originals, X1 split 0.50 vs X2 (X2's irreversible loss vs
X1's stronger machine voice, "I thought soap was soap"). The
critic's revisions beat the originals decisively (0.70 each), which
settles the reframe-over-check question.

Winner vs stock baselines: X2 beat B1 (fern/orchid) 0.70, B2 (wrong
report) 0.65, and split B3 (woke baby) 0.50 — mean 0.617, clearing
the 0.60 bar. X4's baseline mean was 0.65, but X2 won the
head-to-head and is shorter (188 vs 203 bytes), so X2 takes the
smaller-text tie-break too.

## Winner

188 characters, 188 bytes, no trailing newline:

```text
I'm sorry I pruned the rose bush the day before it bloomed and cut off every bud.
I have learned a bud is next week's flower, not clutter to tidy, and now I leave any stem with buds alone.
```

Critic's objections answered: S2 is now a reframe ("a bud is next
week's flower, not clutter to tidy") whose behaviour ("leave any
stem with buds alone") is the application of that reframe, not a
generic check; D1 retired (its tablet-drawer behaviour lives inside
the A3 revision); A2/A4 retired outright.
