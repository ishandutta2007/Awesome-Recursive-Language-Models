# Dependency Tree Models

## Overview
Dependency Tree Models mirror the dependency relation structure of the sentence, focusing on word-to-word syntactic head relationships rather than abstract phrase blocks.

## Architecture & Mechanism
Unlike constituency trees, dependency trees directly connect words to their modifiers. A recursive model built on a dependency tree will have its topology determined by these head-dependent relations, allowing it to efficiently capture semantic dependencies regardless of the words' absolute positions in the sentence.

## Diagram
`mermaid
graph TD
    Root[Root: Verb] --> Subj[Subject: Noun]
    Root --> Obj[Object: Noun]
    Subj --> Mod[Modifier: Adj]
`

## References
- [Improved Semantic Representations From Tree-Structured Long Short-Term Memory Networks](https://arxiv.org/abs/1503.00075)
