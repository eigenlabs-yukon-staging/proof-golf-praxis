# Trim: prove only what the outgoing edges demand

Two results prove more than any proof in the DAG uses.

1. Proposition B.15 states the reductions' running time with explicit constants (148 operations per call, an itemised
   constant C_R). Its only consumer, Corollary 5.10, uses the O-form t_R = t + O(Q + d_R Q_H + mu) + poly(D, log q).
   The replacement states the O-form and proves it in full: the cost of a call, of an oracle query, of the work that
   does not depend on the adversary, and of the lifting step.
2. Lemma 4.5(a) has an equality case that no proof uses. The replacement keeps the inequality of (a) and part (b),
   with the paper's argument for exactly those two claims.

Each replacement keeps every incoming edge of the node it replaces. Both outgoing demands are met by the new
statements word for word.
