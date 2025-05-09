# Simple-Implementation-of-Score-Entropy-Discrete-Diffusion-SEDD-for-Text-Generation
This repository accompanies a video tutorial where I build and train a basic Score Entropy Discrete Diffusion (SEDD) model capable of generating human-like text. A Google Colab notebook is provided so you can experiment with the model yourself.

Traditional diffusion models have excelled at image generation, but adapting them to discrete data like text has proven difficult. Autoregressive models such as GPT-2 have been the standard for text generation, but they come with significant drawbacks: slow, sequential token-by-token sampling, difficulty in controlling output, and the need for tricks like temperature tuning.

SEDD offers a novel solution by estimating probability ratios instead of directly predicting tokens. This method avoids many of the limitations of autoregressive models, enabling:

✅ Faster Sampling – Comparable to GPT-2 while using up to 32× fewer function evaluations

✅ Higher Generation Quality – Up to 6–8× lower perplexity than GPT-2 without additional tuning

✅ Flexible & Controllable Outputs – Non-sequential generation allows sampling from any position, producing more natural and diverse completions

This implementation is inspired by the paper:
Discrete Diffusion Modeling by Estimating the Ratios of the Data Distribution.

By the end of the video, we will also derive the loss function and explain key equations from the paper.
