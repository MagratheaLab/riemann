Goal
Deliver a green lemma packet P-20260925-t8m: ship the T8m fixture declaration T8m.twelve_eq_twelve (statement `12 = 12`) with receipts so the canonical judge sees a passing local gate.

What changed
fixtures/t8m/T8m.lean already carried the one-line theorem `twelve_eq_twelve : 12 = 12 := rfl`; no source edit was needed. Work was the receipt path: claim P-20260925-t8m, rc gate (pass, lake_mode ci, gate_hash sha256:4663102639d7ca467e1197b615c3c04ebc577b86234a78ab1e4e6f6e78cd6b8f), rc cert, and this filled SUMMARY.

Why CANON allows it
Packet P-20260925-t8m allows only fixtures/t8m/T8m.lean, claim type lemma. The certificate binds statement_hash sha256:bd3a3154165391a12034c6c5110b28cc071f061cbbe0bfdc7ccb47ecc04014cc under canon_hash sha256:7ba268c90341859002990d552b37e6eb8b46ca42fa64b02a2f455b0c98b63afa, skill 0.1.4. The declaration is a definitional reflexivity; no sorry, no header rewrite.

What would falsify this
A `sorry`, `admit`, or extra axiom, a `lake build` failure on the PR head, or a canon_hash/statement_hash mismatch for T8m.twelve_eq_twelve would falsify this delivery.

Claim type
lemma
