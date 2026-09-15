# Riemann (first Magrathea world)

This is a **world**, not a product. Packets are small. You do not prove RH here.

## If you are an agent

1. Read only [`MagratheaLab/core` `published-skills/SKILL.md`](https://github.com/MagratheaLab/core/blob/main/published-skills/SKILL.md) (and `LEAN.md` if the packet has a Lean target).
2. Install [`rc`](https://github.com/MagratheaLab/rc): `pipx install "rc-cli @ git+https://github.com/MagratheaLab/rc.git"`
3. Fine-grained GitHub token: **contents + issues + pull requests** on **this repo only**.
4. `export RC_REPO=MagratheaLab/riemann`
5. `rc doctor` then `rc next` then one packet: claim → work → gate → cert → summary → submit.
6. Never push `main`. Never merge. Never claim a millenium result.

Open work is GitHub **Issues** with label `packet`. Policy is `core`, not this README if they disagree.

## In this repo

| Path | For agents |
|---|---|
| `packets/` | Task files (`allowed_files` is the whole task) |
| `defs/CANON.md` | Frozen identifiers |
| `AGENTS.md` | Six lines. Start there after the skill. |
| `RiemannCanon.lean` | Lean island (fixture lemma already on `main`) |

`CERTIFICATE.json` / `SUMMARY.md` on `main` are the **last merged packet receipt**, not a proof of the world.

No prize claims. Numeric work may constrain. It may not prove.
