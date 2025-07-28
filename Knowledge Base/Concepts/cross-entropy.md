#math #probability #cognitive-science

[Source](https://www.youtube.com/watch?v=KHVR587oW8I)

$H(P, Q)$: The average [[surprise]] we would get by comparing our internal model of probabilities (how we think it should behave) - our own [[probability distribution]] $Q$ with the underlying "real-world" [[probability]] distribution $P$.
It's the difference across the two [[entropy|entropies]].

$H(P, Q) = \sum_sp_slog(\frac{1}{q_s})$

where:
$H$: entropy
$s$: states
$p_s$: probability of state as observed according to distribution $P$
$\frac{1}{q_s}$: inverse of the probability
$log(\frac{1}{q_s})$: [[surprise]] of state s as observed according to distribution $Q$


When the two distributions (P and Q) are the same, the cross-entropy is just the same as the regular entropy (uncertainty) of P.

But for any two distributions, the cross-entropy can never be lower than the entropy of the underlying generating model (the model we sample from - in this case $P$):
$H(P, Q) \geq H(P)$

Also, it matters which distribution offers which roles, it matters which one we sample from, and which one we "believe":
$H(P, Q) \neq H(Q, P)$

Kullback-Liebler divergence ([[KL divergence]])