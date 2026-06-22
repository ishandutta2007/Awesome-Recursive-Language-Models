# Mathematical Formula Evaluation

## Overview
Mathematical expressions are highly structured and strictly obey the order of operations, making them a perfect use case for recursive models.

## Architecture & Mechanism
Symbolic computation and automated theorem proving engines rely on recursive language models to evaluate complex algebraic expressions or execute parenthetical logic tracking without breaking order-of-operation constraints. A recursive network naturally follows the computation graph of the formula.

## Diagram
`mermaid
graph TD
    Add[+] --> Mul[*]
    Add --> Num3[3]
    Mul --> Num1[1]
    Mul --> Num2[2]
`

## References
- [Neural Equivalence Networks](https://arxiv.org/abs/1611.00711)
