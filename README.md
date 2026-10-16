# PolicyMoE pilot results

This repository publishes a small, source-grounded PolicyMoE experiment inspired by the [PolicyLLM paper](https://arxiv.org/abs/2604.12995).

## What is included

- 150 questions built from 25 public U.S. Department of Energy policy documents
- a document-grouped split: 100 training questions and 50 questions from five held-out documents
- a frozen Qwen2.5-7B-Instruct baseline
- one LoRA trained on all levels
- three level-specific LoRA experts and a learned linear top-1 router
- predictions, metrics, router history, sample questions, and a public results page

## Main result

On 43 objective held-out questions, PolicyMoE matched the single-LoRA model and did not outperform the frozen baseline overall. Seven open-ended Level 3 questions remain unscored because the two-model judging stage was not configured. This is an execution pilot, not a reproduction of the paper’s full benchmark or evidence of architecture superiority.

View the published page: <https://ywang2622.github.io/policy-moe-smoke-results/>
