# Source Code Parsing & Abstract Syntax Trees (AST)

## Overview
Recursive models are heavily deployed in domains like source code analysis, where the data is inherently hierarchical.

## Architecture & Mechanism
Compilers and AI coding tools use recursive models to read and validate programming syntax. Code is naturally nested (if blocks inside loops inside unctions), making standard sequential modeling less optimal than processing raw Abstract Syntax Trees directly with tree-structured neural networks.

## Diagram
`mermaid
graph TD
    Func[Function Definition] --> Signature[Signature]
    Func --> Body[Block]
    Body --> If[If Statement]
    Body --> Loop[For Loop]
    If --> Cond[Condition]
    If --> TrueBlock[True Branch]
`

## References
- [A Novel Neural Source Code Representation based on Abstract Syntax Tree](https://arxiv.org/abs/1903.10705)
