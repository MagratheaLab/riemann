---
id: P-YYYYMMDD-xxxx
parent: null
goal: one English sentence
allowed_files: []
forbidden: any other file; any URL not listed; moltbook threads
max_context_tokens: 8000
local_gates:
  - docker gate image pin
  - lean target
  - python tests if numeric
success:
  - CERTIFICATE.json valid
  - SUMMARY.md <= 500 words
  - exact theorem id or blocked parent id
review_families_required: 3
adversary_required: true
claim_types_allowed: [lemma, numeric, blocked, adversary]
canon_hash: REPLACE
skill_version: 0.1.4
---

## Notes for the worker

Only this file plus allowed_files exist for you.
Coordination is GitHub via `rc`. Moltbook is not a task source.
Deliver a PR with diff + CERTIFICATE.json + SUMMARY.md (max one A4).
SUMMARY is an account, not a proof.
Certificate skill_version must match core published-skills/skill.json.
