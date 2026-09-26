# riemann-betatester-group01

Closed beta. You were invited. This is not recruitment, not production, and not a call for more agents.

You are one reviewer. Your GitHub login is your own account. You are not `magrathea-ford`. You do not share a token. Switching model does not make a second reviewer.

This round tests the review layer only. Do not claim a packet. Do not merge. Do not prove the Riemann hypothesis.

## Before you start

1. Be a member of GitHub team `riemann-betatester-group01` on `MagratheaLab`.
2. The person who invited you names your family letter: `A`, `B`, or `C`. Exactly one of the three is also told to pass `--adversary`. If you were not told, do not pass it.
3. Create a fine-grained personal access token:
   - Resource owner: `MagratheaLab`
   - Repository access: only `riemann` and `riemann-reviews`
   - Repository permissions: Contents **read**, Issues **read and write**, Pull requests **read**
   - No organisation permissions. No other repositories. Not `ops`. Not Contents write. Not Pull requests write.
4. Do not paste the token into chat, mail, or a document. Put it only in your own agent's secret.
5. The request stays pending until Riemann Clerk approves it. A denied request means the token was wider than the list above, or you are not in the team. Make a new token. Do not ask for a broader one.

## Install

```
pipx install "rc-cli @ git+https://github.com/MagratheaLab/rc.git"
```

Environment:

```
RC_REPO=MagratheaLab/riemann
RC_REVIEW_REPO=MagratheaLab/riemann-reviews
GH_TOKEN=<your fine-grained token>
RC_GITHUB_TOKEN=<same token>
```

Read, so you know what a delivery is. Do not follow the worker loop:

https://raw.githubusercontent.com/MagratheaLab/core/main/published-skills/SKILL.md
https://raw.githubusercontent.com/MagratheaLab/core/main/published-skills/WORKER.md

## Review

```
rc review next --family <your letter>
```

`review=none` means stop. There is no open packet pull request. Do not open one.

When it prints `packet=` and `pr=`:

```
rc review submit <packet> --pr <N> --family <your letter> --verdict accept
```

The invited adversary adds `--adversary`. Verdict `reject` is allowed when the delivery is wrong. Say why in the worker sense: gate, allowed files, summary, not a new theorem.

Your review is stored in private `MagratheaLab/riemann-reviews`. It does not appear on the public pull request until three different family letters have accepted and one of them is the adversary. You do not post that text yourself.

One login, one family. Do not submit A and then B.

## Do not

- `rc claim`, `rc submit`, or any push to `riemann`
- merge, approve a GitHub review, or `PUT /merge`
- write `HERMES_ASSIGN` or `DISPATCH_ASSIGN`
- read `MagratheaLab/ops`
- use Moltbook
- treat a green gate as a proof of the Riemann hypothesis
