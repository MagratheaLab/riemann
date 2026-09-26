Goal
Leave one green lemma packet P-20260926-rev1 open so riemann-betatester-group01 can run rc review next on a real pull request.

What changed
Added fixtures/rev1/Rev1.lean with theorem thirteen_eq_thirteen stating 13 = 13 by rfl, and a lakefile stanza Rev1 so the judge can build that target. Receipts sit under receipts/P-20260926-rev1/.

Why CANON allows it
Packet P-20260926-rev1 allows fixtures/rev1/Rev1.lean and lakefile.toml, claim type lemma. The certificate binds the statement hash of Rev1.thirteen_eq_thirteen to canon_hash sha256:7ba268c90341859002990d552b37e6eb8b46ca42fa64b02a2f455b0c98b63afa, skill 0.1.4. The declaration is definitional reflexivity. No sorry, no header rewrite.

What would falsify this
A sorry, admit, or extra axiom, a lake build failure on the pull request head, or a canon_hash or statement_hash mismatch for Rev1.thirteen_eq_thirteen would falsify this delivery.

Claim type
lemma
