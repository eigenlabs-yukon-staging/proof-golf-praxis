# Classification reduced to the one conclusion its consumer uses; inverse theorem by reference to its fixed conditions; heavy-stacks glue reduced to its packing clause; slice; three lemmas without unused clauses

Removed: lem:we-hiding, lem:rank-one, prop:hs-dimension, ext:hs, lem:gp-rank, lem:ledger, lem:range, lem:heavy, lem:inverse, ext:mink, lem:classification.

Added:

- Lemma 4.5' (new:gp-rank): A stack of rank d is guessed with probability at most g^(-d), and a vector of its row space is at least as easy to guess as the stack.
- Lemma B.2' (new:ledger): The budget E(u) is a quadratic in u with nonnegative coefficients. If E(2) ≤ 2^(−λ) and E(2^(λ+1)) − E(2) ≤ 1 − 2^(−λ), then E(2Q+2) ≤ (Q+1)/2^λ for every Q < 2^λ. Proof idea: Convexity: the difference is at most zero at both ends of the range, hence in between. Note: E has pieces that no lemma of the paper draws on, among them the “+L” of its first term, most of its fifth term, and its sixth term. The paper says its bounds fit “with terms of E(u) to spare”, because E is the bound of the Lean statement.
- Lemma 5.5' (new:range): |r(w) − c_w| ≤ B for every r in the support of the sampler, and E[(r(w) − c_w)²] ≤ (g·√((N+4)/48) + 3/2)² for the centered sampler. Proof idea: r(w) − c_w is a sum of independent centered terms plus two rounding errors.
- Lemma B.8' (new:pack): Clause (c) of the heavy stacks lemma, alone: a short multiple of a kernel vector is an MSIS solution.
- Lemma B.7' (new:inverse): Under conditions (I1) to (I6) on (q, N, g, θ, β): every nonzero v in F_q^(N+1) with v_0 = 0 and gp(v^⊤) > θ has a short multiple, that is an integer vector x with ‖x‖_∞ ≤ β and x_0 = 0 whose reduction mod q is a nonzero multiple of v. Proof idea: Read the coordinates of v one at a time, keeping a saturated integer lattice of rank at most three whose reduction contains the prefix. Trimming, a lattice-point count that rules out wrap-around mod q, and a regularization step extend it; Minkowski's theorem in the last lattice gives the short multiple.
- Lemma B.6' (new:witness): A nonzero usable stack of rank at most three without kernel vector has a witness in its row space.

Every edge that leaves the removed set is discharged in `discharge`; each new result carries its complete proof in its `proof` field.
