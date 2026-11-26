# Slice; rank bound, generic bound and search range each without the clause no proof uses

Removed: lem:we-hiding, lem:rank-one, prop:hs-dimension, ext:hs, lem:gp-rank, lem:ledger, lem:range.

Added:

- Lemma 4.5' (new:gp-rank): A stack of rank d is guessed with probability at most g^(-d), and a vector of its row space is at least as easy to guess as the stack.
- Lemma B.2' (new:ledger): The budget E(u) is a quadratic in u with nonnegative coefficients. If E(2) ≤ 2^(−λ) and E(2^(λ+1)) − E(2) ≤ 1 − 2^(−λ), then E(2Q+2) ≤ (Q+1)/2^λ for every Q < 2^λ. Proof idea: Convexity: the difference is at most zero at both ends of the range, hence in between. Note: E has pieces that no lemma of the paper draws on, among them the “+L” of its first term, most of its fifth term, and its sixth term. The paper says its bounds fit “with terms of E(u) to spare”, because E is the bound of the Lean statement.
- Lemma 5.5' (new:range): |r(w) − c_w| ≤ B for every r in the support of the sampler, and E[(r(w) − c_w)²] ≤ (g·√((N+4)/48) + 3/2)² for the centered sampler. Proof idea: r(w) − c_w is a sum of independent centered terms plus two rounding errors.

Every edge that leaves the removed set is discharged in `discharge`; each new result carries its complete proof in its `proof` field.
