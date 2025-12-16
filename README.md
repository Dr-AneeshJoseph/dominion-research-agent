# 🌳 D.O.M.I.N.I.O.N. (Research Agent)

> **The Tree-of-Thoughts Engine for Ambiguous Problems.**

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## ⚠️ The Problem
Standard Agents converge too fast. If you ask a broad question, they grab the first probability token and run with it, often missing the best solution.

## 🛡️ The Solution
**D.O.M.I.N.I.O.N.** implements **Loop 3 (Branching)**.
It forces the model to generate 5-9 distinct hypotheses first.
Then, it uses a Python "Pruner" to kill the weak ideas and only execute the strongest 2 paths.

## 🚀 Quick Start
```python
from dominion.pathfinder import DominionPathfinder
# See examples/market_research_demo.py
