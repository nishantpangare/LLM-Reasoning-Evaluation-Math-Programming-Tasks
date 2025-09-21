# LLM-Reasoning-Evaluation-Math-Programming-Tasks
This project implements and evaluates reasoning pipelines for Large Language Models (LLMs) on mathematics and programming tasks. The goal is to explore step-by-step reasoning, self-consistency, and error analysis for improving the correctness and transparency of LLM outputs.


**Project Overview**

Built an evaluation framework for reasoning in LLMs using Hugging Face transformers.

Designed Chain-of-Thought (CoT) prompts for math problems and function generation prompts for programming tasks.

Compared Greedy Decoding vs. Self-Consistency sampling strategies.

Developed verifiers to check numeric answers (math) and run unit tests (programming).

Collected results in .csv files for systematic analysis and reporting.



**⚙️ Technical Toolkit**

Python – core implementation

Hugging Face Transformers – model inference (flan-t5-large)

PyTorch – backend for model execution

pandas / csv – results storage & analysis

tqdm – progress tracking

Regex & unit testing – answer/code verification


**📊 Results Summary**

Math Tasks

Greedy accuracy: 30%

Self-consistency accuracy: 40%

Common errors: arithmetic mistakes, skipped steps, hallucinations.

Programming Tasks

Greedy success: 0%

Self-consistency success: 0%

**Common errors:** incomplete functions, missing returns, and logical mistakes.

**Self-consistency helped in math but failed in programming → showing limits of Flan-T5-XL for structured reasoning.**
