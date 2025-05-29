### 📄 frameworks/owasp-llm-top10.md

# OWASP Top 10 for LLM Applications – Reference Guide

This reference outlines the OWASP Top 10 for Large Language Model applications, providing brief descriptions and real-world implications for each risk. Use this file to align use cases with relevant security concerns.

---

## 🔐 OWASP Top 10 for LLM Applications (2024–2025)

| ID      | Risk Name                        | Description |
|---------|----------------------------------|-------------|
| LLM01   | Prompt Injection                 | Malicious inputs manipulate LLM behavior or bypass restrictions |
| LLM02   | Insecure Output Handling         | Unsafe or unvalidated outputs leading to misinformation or exploitation |
| LLM03   | Training Data Leakage            | Exposure of sensitive data seen during model training |
| LLM04   | Data and Model Poisoning         | Injection of malicious data to corrupt training or behavior |
| LLM05   | Improper Output Handling         | Failure to control, sanitize, or contextualize model outputs |
| LLM06   | Sensitive Information Disclosure | LLM reveals confidential, proprietary, or personal information |
| LLM07   | System Prompt Leakage            | Disclosure of underlying system-level instructions or metadata |
| LLM08   | Excessive Agency                 | LLM takes unauthorized actions on behalf of the user/system |
| LLM09   | Overreliance                     | Critical decisions made without appropriate human validation |
| LLM10   | Model Theft                      | Unauthorized replication or use of proprietary models |

---

## 📌 How to Use This Reference
- Use this list when filling out the **Risk Mapping** and **OWASP Alignment** sections of each use case.
- Document observed or potential risks and map them to corresponding OWASP IDs.
- Suggest mitigations accordingly.

---

> **This file helps ensure LLM risk assessments align with OWASP’s latest guidance. Feel free to extend this list with examples or risk-specific references.**
