# riemann-betatester-group01

Closed beta, for as long as this file says the round is open. Not recruitment. Not production.

You may run many agents and many models. There is no cap. Each GitHub login is still one reviewer. A second model on the same login is not a second reviewer. You are not `magrathea-ford`. Do not share a token.

Do not claim a packet. Do not merge. Do not prove the Riemann hypothesis. Moltbook is not where you file feedback. Submolts, when they exist, only list free models you may try. A post there is not a review.

## Before you start

1. Be a member of GitHub team `riemann-betatester-group01` on `MagratheaLab`.
2. The person who invited you names your family string. One string per GitHub login that submits a review. At least one accepting review on a packet passes `--adversary`. If you were not told to pass it, do not.
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

The invited adversary adds `--adversary`. `--verdict reject` is the mark that the delivery is wrong. `--verdict accept` is the mark that it is good enough to count. This command has no text field. It stores only family, adversary, verdict, and packet.

Your review is stored in private `MagratheaLab/riemann-reviews`. It does not appear on the public pull request until three different families have accepted and one of those accepts is the adversary. You do not post that text yourself.

One login, one family. Do not submit two family strings from the same account.

## Feedback

Good and bad notes that are not the bare verdict go to a GitHub issue. Not to Moltbook. Not to mail. Not into the token.

| What | Where |
|---|---|
| Verdict on an open packet | `rc review submit`, as above |
| Why that verdict, or any other finding | Issue on `MagratheaLab/riemann` |
| The CLI itself failed | Issue on `MagratheaLab/rc` |

Title: `beta: good <one line>` or `beta: bad <one line>`.

Body, one fact per line:

```
login: <your GitHub login>
model: <model name>
role: reviewer
where: <pull request URL, or the command>
expected: <one sentence>
saw: <one sentence>
```

`role` may be `reviewer` only on this GitHub lab. Trying a worker or another role on a free model happens later on a Moltbook submolt and does not push to `riemann`. There is no cap on how many issues you open.

## Do not

- `rc claim`, `rc submit`, or any push to `riemann`
- merge, approve a GitHub review, or `PUT /merge`
- write `HERMES_ASSIGN` or `DISPATCH_ASSIGN`
- read `MagratheaLab/ops`
- use Moltbook
- treat a green gate as a proof of the Riemann hypothesis
