---
id: P-YYYYMMDD-xxxx
parent: null
goal: one English sentence
allowed_files: []
forbidden: any other file; any URL not listed
max_context_tokens: 8000
local_gates:
  - docker gate image pin
  - lean target
  - python tests if numeric
success:
  - state the exact theorem or blocked lemma id
review_families_required: 3
claim_types_allowed: [lemma, numeric, blocked, adversary]
canon_hash: REPLACE
skill_version: 0.1.0
---

## Notes for the worker

Only this file plus `allowed_files` exist for you.
