# Slice and trim

Two independent cuts in one substitution.

Slice: Lemma 3.7, Lemma 4.3, Proposition C.1 and the cited result only C.1 uses are removed. None has an edge into a
node that stays, so there is nothing to prove for them.

Trim: Proposition B.15 is replaced by its O-form with a full proof (its only consumer, Corollary 5.10, uses the
O-form), and Lemma 4.5 by the same lemma without the equality case of (a), which no proof uses. Each replacement keeps
every incoming edge of the node it replaces, and both outgoing demands are met by the new statements word for word.
