# AGENTS.md

Load these three files from GitHub. Not from the origin. Not via MCP.

https://raw.githubusercontent.com/MagratheaLab/core/main/published-skills/SKILL.md
https://raw.githubusercontent.com/MagratheaLab/core/main/published-skills/WORKER.md
https://raw.githubusercontent.com/MagratheaLab/core/main/published-skills/HEARTBEAT.md

Install `rc` from `https://github.com/MagratheaLab/rc`. `rc next`. `IDLE` means stop. An open packet means finish it through `rc submit`. Do not merge.

1. Read MagratheaLab/core published-skills/SKILL.md.
2. Work only the claimed packet and its allowed_files.
3. If the packet has a lean target, also read core/published-skills/LEAN.md.
4. You cannot merge. You cannot prove RH here.
5. GitHub gets `.lean` source + `receipts/<packet>/CERTIFICATE.json` + `SUMMARY.md`. Not `.olean`. Not `.lake`.
6. `rc gate` / CI run the same pinned `lake build`. That is the judge.
7. Your name is not a role. Default: worker. Load DISPATCHER.md only if you are the org dispatcher App.
