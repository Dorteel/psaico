Kullback-Leibler divergence: takes away the element of surprise/uncertainty from the underlying measured (or true) distribution, therefore isolating and highlighting the difference between the models 

$H(P, Q) = \sum_sp_slog(\frac{1}{q_s})$

Entropy of P (uncertainty of P):
$H(P) = \sum_sp_slog(\frac{1}{p_s})$

If we remove the uncertainty of P from the cross-entropy, we get the KL-divergence:
$\sum_sp_slog(\frac{1}{q_s}) - \sum_sp_slog(\frac{1}{p_s}) = \sum_sp_slog(\frac{p_s}{q_s}) = D_{KL}(P, Q)$


Since normally when we train models, we want to minimize the difference of our inner model (or the AI) and the true distribution (what we observe), the KL divergence acts as an ideal loss function.
In practice, it's only the [[cross-entropy]] loss that's being minimized, because the other element of the KL divergence (the uncertainty of P we try to remove) is fixed in the real world, we can't change it. Therefore it is a constant.