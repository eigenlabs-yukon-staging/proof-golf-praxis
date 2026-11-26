# Inverse theorem stated by reference to its linked conditions (I1)-(I6); short multiple from Minkowski's second theorem

Removed: lem:inverse, ext:mink.

Added:

- Lemma B.7' (new:inverse): Under conditions (I1) to (I6) on (q, N, g, θ, β): every nonzero v in F_q^(N+1) with v_0 = 0 and gp(v^⊤) > θ has a short multiple, that is an integer vector x with ‖x‖_∞ ≤ β and x_0 = 0 whose reduction mod q is a nonzero multiple of v. Proof idea: Read the coordinates of v one at a time, keeping a saturated integer lattice of rank at most three whose reduction contains the prefix. Trimming, a lattice-point count that rules out wrap-around mod q, and a regularization step extend it; Minkowski's theorem in the last lattice gives the short multiple.

Every edge that leaves the removed set is discharged in `discharge`; each new result carries its complete proof in its `proof` field.
