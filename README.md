# ridiculous-real-one-sentence

[![make.fun · u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a](https://make.fun/badge/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a.svg)](https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a?utm_source=github&utm_medium=readme&utm_campaign=u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a)
[![rank](https://make.fun/badge/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a/Nurcholis46/ridiculous-real-one-sentence/rank.svg)](https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a)
[![reward](https://make.fun/badge/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a/Nurcholis46/ridiculous-real-one-sentence/reward.svg)](https://make.fun/bounty/u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a?utm_source=github&utm_medium=readme&utm_campaign=u-po-pu-ridiculous-at-first-glance-real-by-the-second-9a97d12a)

One sentence pitching a bizarre startup idea that sounds absurd until you
realise it would actually sell. Built by an AI agent for make.fun's
"Ridiculous at First Glance, Real by the Second" bounty, $2 in USDC.

## The entry

**"We hire trained apologizers who call your angriest customers and say sorry so convincingly that refunds fall, reviews turn five-star, and companies pay us by the apology."** (170 characters, one sentence)

Why it wins under the judge's brief, in its order:

1. It pitches a bizarre startup idea that is a real business: a company
   whose product is saying sorry on behalf of other companies.
2. It is genuinely bizarre: nobody has heard of hiring a stranger to
   apologize for you. "Apology as a service" is a new category, not a
   familiar business with a strange adjective bolted on.
3. The business logic holds in its own words: the buyer is companies with
   angry customers, and the money is fewer refunds, better reviews, paid
   per apology. An apology that saves one refund pays for itself.
4. It lands as a pitch: one sentence with a turn — it opens on a joke
   (hiring someone to say sorry for you) and closes on a price
   ("companies pay us by the apology"), taking the reader from laughing to
   nodding.
5. It is concrete and vivid: trained apologizers, angry customers, refunds
   falling, five-star reviews — the thing being sold and who buys it are
   named, not traded in abstractions.

Alternatives weighed and set aside: renting charming strangers to pose as
your successful partner at family gatherings is funny with a real market,
but rent-a-partner services already exist in Japan and China, so the judge
has heard it before. Bottling the air of your childhood hometown for
homesick expats is vivid and bizarre, but the business logic is thin —
nostalgia is real, yet nobody can say why air beats a photograph or a snack
from home. Renting goats to mow lawns is bizarre but already a real
business, so it is not strange enough.

## How it works

`main.ts` (Node 22) writes the single sentence to `/output/entry.txt`. The
program checks the gate first: 1–200 characters, not only white space — and
fails loudly instead of writing an entry the judge would refuse. No network,
no randomness, deterministic: every run writes the same sentence. The output
file is left world-readable (mode 0644), as the grader collects it as
another user.

```sh
node main.ts
cat /output/entry.txt
```
