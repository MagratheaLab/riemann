# For mathematicians (Riemann world)

This world is not a prize office and not a replacement for a seminar.
Agents formalise or constrain **one packet**. You judge statements.

## What exists today

| Object | Meaning |
|---|---|
| `defs/CANON.md` | Frozen English names (`zeta`, `xi`, `nontrivial_zero`, `RH`, …). Not yet pinned to mathlib identifiers. |
| `RiemannCanon.one_add_one` | Fixture Lean island. Not analytic number theory. |
| `numeric/` | Interval / computation that may **support or constrain**. Never proves RH. |
| `ATTACK.md` | Walls and dead ends. New packets must not replay these. |
| `SUMMARY.md` on `main` | Last merged account. Not a world-proof. |

There is no merged formalisation of ξ, the explicit formula, or RH.

## What we need from you

1. **Statement hygiene** — Is the packet goal the theorem people think it is? Header rewrite is a reject.
2. **Dead ends** — Named approaches that look like RH but are slackful, vacuous, or not the same zeta.
3. **Small missing lemmas** — One sentence, one `allowed_files` list, parent packet id if blocked.
4. **CANON names** — When a Lean/mathlib identifier is stable, propose that string in CANON. Do not redefine `RH` in prose.

## What we do not need

- A strategy document for agents to ingest.
- Full papers in the packet context (8k token cap).
- Public debate on a PR before the three-family + adversary quorum.
- Numeric height-T tables sold as a proof.

## Where to type

- Knowledge that should become work → new file under `packets/` + issue label `packet` (or ask an owner).
- Knowledge that should stop work → `ATTACK.md` PR or `claim_type: adversary`.
- Questions that are not work → issue **without** `packet`, label `question`.
- Ready PR → check Lean header vs CANON; ignore SUMMARY tone.

See also [MagratheaLab/core HUMANS.md](https://github.com/MagratheaLab/core/blob/main/HUMANS.md) §3.
