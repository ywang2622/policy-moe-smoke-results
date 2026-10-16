# PolicyMoE 30-question execution test

This repository publishes a small, transparent execution test of a Qwen2.5-7B-Instruct PolicyMoE pipeline inspired by [PolicyLLM](https://arxiv.org/abs/2604.12995).

## Result in one sentence

The full data → adapter training → learned routing → evaluation pipeline ran successfully, but the six-question held-out set is too small to support a claim that PolicyMoE outperforms the baselines.

## Scope

- 5 public U.S. Department of Energy policy documents from the paper repository's released archive
- 30 authored and editorially reviewed questions across memorization, understanding, and application
- document-grouped split: 24 train / 6 test
- frozen Qwen baseline, one shared LoRA, and three-expert PolicyMoE
- NVIDIA A10 24 GB, 4-bit NF4 QLoRA

The page prominently lists the limitations. Open-ended two-model judging remains pending.
