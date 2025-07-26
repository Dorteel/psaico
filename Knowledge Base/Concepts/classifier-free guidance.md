**Classifier-Free Guidance (CFG)** is a clever trick in generative models—especially diffusion models—that helps them produce outputs that _better match your prompt_ without needing a separate classifier to nudge them around.

Improving prompt control by subtracting “no prompt” predictions from “prompted” ones.

**In text-to-image models (like Stable Diffusion), CFG does this:**
1. **Generate two outputs:**
    - One with your text prompt (_conditioned_).
    - One with no prompt at all (_unconditioned_).
2. **Blend them:**
    - Final prediction = **unconditioned_output + scale × (conditioned_output – unconditioned_output)**
That subtraction isolates the _effect_ of the prompt, then boosts it with a multiplier (usually 1 to 10ish).

---