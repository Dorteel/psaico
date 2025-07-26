It takes any number and maps them to a value between 0 and 1

# Math
σ(x) = 1 / (1 + e^–x)

* x: input (a number)
* [[e]]^(–x): exponential decay
* 1 + e^(–x): shifting the decay upward so we don't divide by 0
* 1 / (1 + e^(–x)): squashing, compresses the input down to a value between 0 and 1