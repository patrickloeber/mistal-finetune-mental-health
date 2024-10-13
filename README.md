**DISCLAIMER**: 

**This guide is purely for educational purposes. The model does not replace real therapy.**

**The prompts and dataset may contain sensitive information related to mental health.**

**If you need emotional support or counseling, you'll find free helplines at [https://findahelpline.com/](https://findahelpline.com/).**

# Build a mental health companion with Mistral

In this guide, you'll learn how to build a mental health companion with Mistral.

The model learns to provide helpful advice and support based on training data that consists of counseling sessions with qualified psychologists.

We follow this approach:

- Dataset: We finetune Mistral 7B on a mental health counseling conversation dataset.
- Fine-tuning: For finetuning, we'll use the Mistral Finetuning API (This tutorial can be followed by being on the free tier).
- Safeguarding: We'll also employ a second LLM as "supervisor", so you can rate the severity of the user problem and can take extra care and further action if needed.

  ## Get Started

  Open [mistral_finetune_mental_health.ipynb](./mistral_finetune_mental_health.ipynb) and follow the notebook.
