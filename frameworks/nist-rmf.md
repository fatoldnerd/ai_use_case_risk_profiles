# AI Use Case Risk Profiles

Welcome to the **AI Use Case Risk Profiles** repository.

This project provides a structured, easy-to-understand mapping of real-world enterprise LLM use cases to relevant risks, mitigations, and governance frameworks such as the NIST AI Risk Management Framework and OWASP Top 10 for LLM Applications.

> **Goal:** Help enterprises, risk teams, and security-conscious leaders better understand the practical implications of deploying LLMs in various workflows.

---

## 📁 Folder Structure

```bash
ai-use-case-risk-profiles/
├── README.md                  # Project overview and instructions
├── use-cases/
│   ├── customer-support.md    # Use case 1: LLM in customer service chatbots
│   ├── contract-review.md     # Use case 2: Legal document summarization
│   ├── code-generation.md     # Use case 3: LLMs used in developer tools
│   └── ...                    # Add additional use cases here
├── templates/
│   └── use-case-template.md   # Markdown template to add your own use cases
├── frameworks/
│   ├── nist-rmf.md            # High-level mapping to NIST AI RMF
│   └── owasp-llm-top10.md     # Mapping to OWASP LLM risks
└── LICENSE                    # Add a permissive license like MIT or CC-BY
```

---

## 🧠 Example Use Cases (in `use-cases/` folder)
Each use case includes:
- **Business Description**
- **LLM Functionality**
- **Risk Mapping** (e.g., prompt injection, hallucination, misuse)
- **Framework Alignment** (NIST RMF, OWASP Top 10)
- **Mitigation Strategies**
- **Security Considerations**

---

## 📄 How to Use
1. Browse the `use-cases/` folder for examples.
2. Use the template in `templates/use-case-template.md` to add your own.
3. Review the `frameworks/` folder to understand how risks align with governance best practices.

---

## ✅ Contributing
This project is ideal for security professionals, risk managers, and AI governance advocates.

Contributions welcome: pull requests, feedback, and additional use cases.

---

## 🛡 License
To allow for reuse and sharing, this project uses the MIT License or Creative Commons (TBD).

---

### 📄 frameworks/nist-rmf.md

# NIST AI Risk Management Framework (AI RMF) – Reference Guide

This guide outlines how enterprise LLM use cases can be aligned with the NIST AI Risk Management Framework's four core functions:

---

## 🔍 Overview
The NIST AI RMF provides a structured approach to managing AI risks and promoting trustworthy systems. It includes four high-level functions:
- **Map**: Understand the context, intended use, and risk landscape.
- **Measure**: Assess, monitor, and document model performance and associated risks.
- **Manage**: Implement risk mitigation strategies.
- **Govern**: Establish structures for oversight, accountability, and improvement.

---

## 📊 Function-by-Function Mapping for LLM Use Cases

### 🗺 MAP
- Define the AI system’s context, including mission/business objectives.
- Identify stakeholders and their expectations.
- Understand potential risks based on domain, users, and deployment method.
- Example: For a legal summarization bot, identify legal counsel as primary users, and risks of incomplete summaries.

### 📏 MEASURE
- Define metrics to evaluate LLM performance (e.g., hallucination rate, latency, bias levels).
- Identify unknowns (e.g., inability to explain why a model made a decision).
- Use red-teaming, audits, and benchmarks to assess behavior.

### 🔧 MANAGE
- Apply controls: prompt guardrails, access limits, logging, feedback loops.
- Assign responsibilities for ongoing risk oversight.
- Continuously improve prompt templates or fine-tuned models.

### 🧭 GOVERN
- Define governance structures for AI oversight.
- Document policies and practices around responsible AI.
- Ensure cross-functional accountability (IT, Legal, Risk, Product).
- Support transparency and reporting (e.g., model cards, decision logs).

---

> **This file serves as a reference to align each use case with NIST AI RMF best practices. Use it when completing the "Framework Alignment" section of your use cases.**
