**Low-Rank Adaptation**
**LoRA** is a method to fine-tune models efficiently by injecting small trainable low-rank matrices into frozen layers.

Instead of updating the whole giant model (which is costly and memory-heavy), LoRA tweaks just a few extra light-weight parameters. Think of it as adding training "hacks" that steer the model without rewriting its brain.