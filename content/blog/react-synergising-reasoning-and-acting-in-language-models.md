---
title: "ReAct: Synergizing Reasoning and Acting in Language Models"
date: 2023-09-11
tags:
  - chatgpt
---

## Summary

A unique feature of human intelligence is the ability to seamlessly combine task-oriented actions with
verbal reasoning, which has been theorized to play an important role in human cognition for enabling self-regulation or strategization and maintaining a working memory. However, current language models are limited to either reasoning or acting, and cannot combine the two.

ReAct is a paradigm proposed to combine reasoning and acting with language models for solving diverse tasks like question answering, fact checking, and interactive decision making.

## In Depth

- It prompts large language models like PaLM to generate both reasoning traces and actions in an interleaved manner. Reasoning helps induce, track, and update plans for acting, while acting allows incorporating external information into reasoning.
- ReAct was tested on question answering (HotpotQA), fact checking (FEVER), text-based games (ALFWorld), and web navigation (WebShop). It outperformed standard prompting, chain-of-thought, and acting-only baselines across tasks.
- On HotpotQA and FEVER, ReAct interacted with Wikipedia to retrieve facts and reduce reasoning errors. Combining ReAct and chain-of-thought performed best to leverage both internal knowledge and external information.
- On ALFWorld and WebShop, one-shot ReAct prompting outperformed imitation learning trained on thousands of demonstrations, with 34% and 10% higher success rates. Reasoning was crucial for goal tracking.
- ReAct increased model interpretability and diagnosability by distinguishing internal vs external knowledge and exposing reasoning traces. It enabled human-in-the-loop policy editing by thought manipulation.
- Limitations include the difficulty of learning complex reasoning and acting from limited demonstrations. Finetuning was shown to help, and scaling up training data could further improve ReAct.

## Further Reading

1. [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/pdf/2210.03629.pdf)

