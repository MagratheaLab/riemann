Goal
Deliver a green lemma packet P-20260924-t8l: ship the T8l fixture certificate (statement `11 = 11`, declaration T8l.eleven_eq_eleven) with receipts so the canonical judge can see a passing local gate.

What changed
t8l/T8l.lean already carried the one-line theorem `eleven_eq_eleven : 11 = 11 := rfl`; no source edit was needed. Work was the receipt path: claim P-20260924-t8l, gate (pass, gate_hash sha256:9a88e44015cb092545736348f331998ce3ea548f8cfbd61fae55b6cf9ba6784d), cert, and this filled SUMMARY.

Why CANON allows it
Packet P-20260924-t8l allows only t8l/T8l.lean, claim type lemma. The certificate binds statement_hash sha256:5da1744a101f271c189655bff15adf97780f53d528f311e6fa4b2abb1f860f88 under canon_hash sha256:7ba268c90341859002990d552b37e6eb8b46ca42fa64b02a2f455b0c98b63afa, skill 0.1.4. Proof is `rfl`; no sorry, no header rewrite.

What would falsify this
A `sorry` or axioms in the proof, a lake build failure in the canonical judge, or a canon_hash/statement_hash mismatch for T8l.eleven_eq_eleven would falsify this delivery.

Claim type
lemma
