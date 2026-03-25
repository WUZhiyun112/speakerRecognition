#  code-r1: Agent-RL Code Generation System

[![Project Status: Active](https://img.shields.io/badge/Project%20Status-Active-success)](#)
[![Framework: VeRL](https://img.shields.io/badge/Framework-VeRL-blue)](#)
[![Algorithm: GRPO](https://img.shields.io/badge/Algorithm-GRPO-orange)](#)

> **Implementation of an Agent-RL Code Generation System Based on the VeRL Framework.**
> This project aims to implement a self-correcting code generation agent using Reinforcement Learning (RL). By leveraging the VeRL framework, the model continuously optimizes its generation policy based on feedback from an isolated code execution sandbox.

🌐 **Project Website & Progress Tracker:** [https://wuzhiyun112.github.io/codeGenerator/](https://wuzhiyun112.github.io/codeGenerator/)

---

## 🎯 Project Abstract
Traditional Large Language Models (LLMs) rely heavily on Supervised Fine-Tuning (SFT) for code generation, which lacks trial-and-error reasoning and logical self-reflection. `code-r1` introduces a closed-loop **Reinforcement Learning** pipeline using the **VeRL** framework:
1. **Generation:** The model generates code along with its Chain-of-Thought (CoT) reasoning.
2. **Execution:** The generated code is evaluated in an isolated sandbox environment (compilation and unit testing).
3. **Feedback:** A Rule-based Reward Model assigns objective scores based on syntax correctness and test execution results.
4. **Optimization:** The GRPO algorithm updates the model's policy, enabling it to learn from execution errors and self-correct.

