Goal
Deliver the T8g fixture (packet P-20260924-t8g, issue MagratheaLab/riemann#45): lean declaration T8g.six_eq_six stays frozen and receipts are produced autonomously by worker magrathea-ford.

What changed
No Lean edit was needed. The fixture file t8g/T8g.lean already contained `theorem six_eq_six : 6 = 6 := rfl`, and the local gate (lake build T8g in the pinned lean-4.33.0 image) passed without modification. Receipts (CERTIFICATE.json + this SUMMARY.md) were generated for packet P-20260924-t8g.

Why CANON allows it
The statement is a reflexivity trivial (6 = 6) with no new axioms, no sorry/admit, no local notation, and no header rewrite of the frozen declaration T8g.six_eq_six. canon_hash sha256:7ba268c90341859002990d552b37e6eb8b46ca42fa64b02a2f455b0c98b63afa, statement_hash sha256:8425b44825f74f54c0ef6974e90dddeb3904e1a45a637a0335c47e54f5ea5aa4.

What would falsify this
A failing `lake build T8g` in the pinned gate image, a rewritten or missing declaration header, the appearance of sorry/admit/axiom/local notation, or a diff touching a file outside t8g/T8g.lean.

Claim type
lemma

Fixture packet. Not RH. SUMMARY is an account, not a proof.
