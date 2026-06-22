# Latent Tree Learning (Unsupervised Tree LMs)

## Overview
Latent Tree Learning models do not receive a pre-computed linguistic tree. Instead, they learn to parse and construct the tree structure dynamically during training.

## Architecture & Mechanism
The model uses a reinforcement learning policy or a continuous relaxation gate (like the Gumbel-Softmax trick or CYK-like algorithms) to discover its own optimal hierarchical parsing tree purely by minimizing a downstream objective, such as next-token prediction loss or classification error.

## Diagram
```mermaid
graph TD
    Loss[Downstream Task Loss] --> Policy[Tree Parsing Policy]
    Policy --> Node1[Learned Sub-tree 1]
    Policy --> Node2[Learned Sub-tree 2]
    Node1 --> T1[Token 1]
    Node1 --> T2[Token 2]
```

## References
- [Learning to Compose Words into Sentences with Reinforcement Learning](https://arxiv.org/abs/1611.09100)
