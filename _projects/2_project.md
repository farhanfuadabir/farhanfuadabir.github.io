---
layout: page
title: Neuro-Symbolic RL Distillation
description: Extracting editable symbolic policies from black-box reinforcement learning agents.
img: assets/img/6.jpg
importance: 2
category: research
related_publications: false
---

During my M.S. I worked on "Neuro-Symbolic Distillation of Reinforcement Learning Agents," a thesis that combines large language models, differentiable logic, and program synthesis.

Key pieces of the stack:

- **LLM-assisted feature carving.** We prompt LLMs with environment specifications and replay buffers to derive semantically rich yet compact feature dictionaries for both visual and continuous observation spaces.
- **Neural-guided symbolic extraction.** A teacher RL policy supervises a differentiable decision list whose structure is constrained by temporal logic templates. Gradient signals and SAT-based pruning work together to find short, human-auditable rules.
- **Editable safety envelopes.** Because the resulting symbolic policies are composed of understandable predicates, domain experts can patch behaviors without retraining the black-box agent.

The framework consistently approximates high-performing RL agents on MuJoCo and gridworld tasks while surfacing what the policy actually attends to—making it a promising fit for safety-critical autonomy.
