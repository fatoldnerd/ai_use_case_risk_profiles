# Use Case: Contract Review Automation

## 📌 Business Description
Legal and procurement teams use LLMs to assist in the review and summarization of contracts. The system highlights key clauses, flags potential risk areas, and suggests standard language for common provisions.

## ⚙️ LLM Functionality
- Text summarization
- Clause classification
- Risk flagging
- Suggestive drafting

## 🔍 Risk Mapping
| Risk Category             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Hallucination            | LLM may fabricate or misinterpret clauses, leading to legal exposure       |
| Prompt Injection         | Input manipulation could cause incorrect extractions or summaries          |
| Sensitive Info Leakage   | Proprietary or third-party contract data may be improperly reused          |
| Overreliance             | Legal decisions made without human review of LLM-generated summaries       |

## 🧩 Framework Alignment
### NIST AI RMF
- **Map:** Understand use context (e.g., contract type, jurisdiction, review phase)
- **Measure:** Track hallucination and false positive/negative rates in flagged clauses
- **Manage:** Implement review workflows and dual-layer validation with humans
- **Govern:** Define responsibility for legal oversight and data retention policy

### OWASP LLM Risks
- LLM01: Prompt Injection  
- LLM02: Insecure Output Handling  
- LLM06: Sensitive Information Disclosure  
- LLM09: Overreliance

## 🛡 Mitigation Strategies
- Embed LLM output into human-in-the-loop review workflows
- Use retrieval-augmented generation (RAG) with vetted clause libraries
- Log and audit all reviews and changes made by the LLM
- Implement guardrails to prevent copying proprietary contract data into prompts

## 🔐 Security Considerations
- Apply encryption and access control to uploaded contracts
- Mask sensitive data where feasible during processing
- Maintain audit logs for external legal compliance or audits

---

> **Last Updated:** May 2025
