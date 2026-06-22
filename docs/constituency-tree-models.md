# Constituency Tree Models (Fixed-Syntax)

## Overview
Constituency Tree Models are a structural variant of recursive networks that rely on an external, linguistic parser (like the Stanford Parser) to generate a static grammatical constituency tree before training begins.

## Architecture & Mechanism
Because the syntax tree is fixed, the recursive network strictly follows the grammatical rules of the language. This behavior makes the model highly interpretable, as each node corresponds to a specific linguistic phrase (e.g., Noun Phrase, Verb Phrase), but it is rigidly bound to strict grammatical syntax rules.

## Diagram
`mermaid
graph TD
    S[Sentence] --> NP[Noun Phrase]
    S --> VP[Verb Phrase]
    NP --> D[Determiner]
    NP --> N[Noun]
    VP --> V[Verb]
    VP --> NP2[Noun Phrase]
`

## References
- [Parsing Natural Scenes and Natural Language with Recursive Neural Networks](https://ai.stanford.edu/~ang/papers/icml11-ParsingWithRecursiveNeuralNetworks.pdf)
