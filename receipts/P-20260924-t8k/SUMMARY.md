Goal
Packet P-20260924-t8k: prove the T8k fixture declaration T8k.ten_eq_ten (10 = 10) in Lean 4 v4.33.0 and deliver the receipts (CERTIFICATE.json + this SUMMARY.md) autonomously. Claim type is lemma; not RH.

What changed
t8k/T8k.lean contains the declaration `theorem ten_eq_ten : 10 = 10 := rfl`; no other file touched. The only diff is the single-rfl proof term.

Why CANON allows it
Packet P-20260924-t8k allows exactly t8k/T8k.lean. statement_hash sha256:ba8ff941a395bd6f91888ece6869a3f838491a76ca25637ca31e4ce79713456f binds the declaration T8k.ten_eq_ten; canon_hash sha256:7ba268c90341859002990d552b37e6eb8b46ca42fa64b02a2f455b0c98b63afa matches the canonical packet. Gate local=pass on lake build T8k with gate image lean-4.33.0.

What would falsify this
A lake build failure of T8k in the canonical gate image, presence of `sorry` in t8k/T8k.lean, any header/declaration rewrite changing T8k.ten_eq_ten, or a statement_hash mismatch against the certificate.

Claim type
lemma
