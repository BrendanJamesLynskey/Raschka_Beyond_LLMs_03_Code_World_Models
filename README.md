# Beyond Standard LLMs 03 &mdash; Code World Models

A companion to Sebastian Raschka's article *[Beyond Standard LLMs](https://magazine.sebastianraschka.com/p/beyond-standard-llms)*. The third of five decks unpacking the four post-transformer architecture families.

This deck takes the **code world model** family: a 32B dense decoder mid-trained on interleaved source code and execution traces, so the model internalises program-state evolution rather than just code text. Matches gpt-oss-20b at parity, exceeds gpt-oss-120b with test-time scaling &mdash; at 4&times; smaller parameter count. The world-modelling mid-training stage is the lever; the architecture is deliberately conservative so the result is methodologically clean.

Includes an **interactive world-model rollout stepper** that runs a small program side-by-side under a standard code LLM (source only) and a CWM (source + state trace + verdict), with a button to inject a bug so you can see the verdict flip from OK to DIVERGED in real time.

**Live site:** https://brendanjameslynskey.github.io/Raschka_Beyond_LLMs_03_Code_World_Models/

## Companion deck series

| # | Deck | Architecture family |
|---|------|---------------------|
| 01 | [Linear-Attention Hybrids](https://brendanjameslynskey.github.io/Raschka_Beyond_LLMs_01_Linear_Attention_Hybrids/) | MiniMax-M1, Qwen3-Next, DeepSeek V3.2, Kimi Linear &middot; gated DeltaNet &middot; KV-cache calculator |
| 02 | [Text Diffusion Models](https://brendanjameslynskey.github.io/Raschka_Beyond_LLMs_02_Text_Diffusion/) | LLaDA, Gemini Diffusion &middot; iterative denoising &middot; diffusion-vs-AR visualiser |
| 03 | [Code World Models](https://brendanjameslynskey.github.io/Raschka_Beyond_LLMs_03_Code_World_Models/) | CWM 32B &middot; world-modelling mid-training &middot; rollout stepper |
| 04 | [Small Recursive Transformers](https://brendanjameslynskey.github.io/Raschka_Beyond_LLMs_04_Small_Recursive_Transformers/) | HRM, TRM &middot; iterative self-loops &middot; recursive trace viewer |
| 05 | [When to Reach for Non-Transformer](https://brendanjameslynskey.github.io/Raschka_Beyond_LLMs_05_Decision_Tree/) | Synthesis &middot; decision-tree walker |

Part of the [Modern Architectures sub-hub](https://github.com/BrendanJamesLynskey/LLM_Hub_Modern_Architectures).
