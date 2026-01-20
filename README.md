Automated Code Review and Optimization Using Large Language Models
Table of Contents

Overview

Repository Structure

Requirements

Running the Analysis

Dataset Overview

Metrics & Analysis

Structural Complexity

Code Quality

Security

Key Findings

Conclusion & Future Work

Authors & Supervisor

Paper Reference


Overview

This repository contains the complete graduation project “Automated Code Review and Optimization Using Large Language Models”, submitted to the Computer Science Department, Jordan University of Science and Technology.

The project implements a structured, multi-dimensional framework for analyzing Python code, comparing Human-written vs AI-generated code (ChatGPT, Google Gemini, GitHub Copilot) across code quality, algorithmic efficiency, and security.

It includes:

The research paper (conference_101719.pdf)

Dataset of Python files (Human & AI-generated)

Python analysis code integrated into a single Jupyter Notebook (مشروع_1_نتائج_ (1).ipynb) for metrics extraction, comparison, and visualization

Repository Structure
AI-Graduation-Project/
├── README.md
├── python_dataset/                 # Extracted dataset
│   ├── open_source/
│   ├── code_smells/
│   ├── algorithms/
│   ├── security/
│   └── ai_generated/
│       ├── open_source/
│       ├── code_smells/
│       ├── algorithms/
│       └── security/
├── مشروع_1_نتائج_ (1).ipynb       # Combined analysis notebook
├── Aggregated_Comparison_Tables.xlsx
├── figures/                        # Paper figures (PNG / JPEG)
├── conference_101719.pdf           # Final paper
├── references.bib                  # Paper references
├── IEEEtran.cls
└── IEEEtran_HOWTO.pdf

Requirements

Install Python dependencies:

pip install pandas numpy matplotlib seaborn openpyxl jupyter

Running the Analysis

Run the Jupyter Notebook for metrics extraction, analysis, and visualization:

jupyter notebook "مشروع_1_نتائج_ (1).ipynb"


Generates:

Code quality metrics

Structural complexity metrics (functions, lines, loops, recursion)

Security evaluation summaries

Visualizations (Boxplots, Bar Charts, Heatmaps)

Aggregated comparison of Human-written vs AI-generated code

Dataset Overview

1️⃣ Open Source (Code Quality)

Path: python_dataset/open_source/

Purpose: High-quality baseline for readability, modularity, naming, documentation, and clean architecture

2️⃣ Code Smells

Path: python_dataset/code_smells/

Purpose: Detect long functions, duplicated code, poor naming, god functions

3️⃣ Algorithms (Time & Space Complexity)

Path: python_dataset/algorithms/

Purpose: Measure efficiency (Big-O), scalability, algorithmic complexity

4️⃣ Security

Path: python_dataset/security/

Purpose: Detect vulnerabilities, injections, unsafe cryptography, hardcoded secrets

5️⃣ AI-Generated Code

Path: python_dataset/ai_generated/ (mirrors the 4 axes above)

Purpose: Compare AI-generated code against Human-written code using same evaluation criteria

Metrics & Analysis
Structural Complexity
Metric	Description
num_functions	Number of functions in file
avg_function_length	Average function size in lines
max_function_length	Maximum function length
loops_count	Number of loops
has_recursion	Recursion usage
total_lines	Total lines of code
Code Quality
Metric	Description
code_score	Quality score out of 100
num_code_issues	Detected code smells or style issues
Security
Metric	Description
security_issues	Number of detected security vulnerabilities
Key Findings

AI-generated code: Consistent style, concise functions, fewer code smells, easier to maintain

Human code: Better algorithmic efficiency, higher modularity, more complex control flow (loops, recursion)

Security: Comparable across both AI and Human code, with static analysis detecting outliers in human projects

Conclusion & Future Work

The framework successfully evaluates Python code using LLMs, combining rule-based static analysis, complexity metrics, and LLM-guided interpretation. AI excels in maintainability and style, while human developers outperform in algorithmic efficiency and control flows.

Future work includes:

Extend dataset with real-world, multi-file repositories and external dependencies

Dynamic benchmarking for execution time and scalability

Sensitivity analysis across prompts, LLM versions, and temperature settings

Integration into CI pipelines for AI-assisted development

Authors & Supervisor

Authors:
Ruba AL Harahshah [158415]
Huda Shqerat [163547]
Hala ALshouha [147651]
Sara Jaradat [165199]

Supervisor: Yaser Jararweh
Faculty of Computer Science and IT, Jordan University of Science and Technology — Jan 2026

Paper Reference

AL Harahshah, R., Shqerat, H., ALshouha, H., Jaradat, S., Jararweh, Y.
“Automated Code Review and Optimization Using Large Language Models,” Final Project Report, JUST, 2026.

License

