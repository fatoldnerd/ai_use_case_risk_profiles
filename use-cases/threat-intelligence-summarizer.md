# Use Case: Threat Intelligence Summarizer

## 📌 Business Description
Security teams use LLMs to summarize threat intelligence feeds, research reports, and internal alerts. The goal is to quickly surface relevant insights, prioritize risks, and support faster decision-making during security incidents or routine analysis.

## ⚙️ LLM Functionality
- Natural language summarization
- Entity recognition (e.g., IOCs, actors, TTPs)
- Contextual Q&A
- Pattern identification

## 🔍 Risk Mapping
| Risk Category             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Hallucination            | LLM may invent threat actors, timelines, or impact scenarios                |
| Insecure Output Handling | Summarized intelligence may omit critical context or misstate urgency       |
| Prompt Injection         | Input from external feeds could manipulate the LLM's interpretation         |
| Sensitive Info Leakage   | Internal alerts or threat reports may be inappropriately surfaced           |

## 🧩 Framework Alignment
### NIST AI RMF
- **Map:** Define intended use (daily triage, board reports, or incident response)
- **Measure:** Evaluate summary accuracy, timeliness, and completeness
- **Manage:** Implement human review before alerts are shared with decision-makers
- **Govern:** Maintain traceability of original sources and review workflows

### OWASP LLM Risks
- LLM01: Prompt Injection  
- LLM02: Insecure Output Handling  
- LLM06: Sensitive Information Disclosure  
- LLM09: Overreliance

## 🛡 Mitigation Strategies
- Require traceable references in LLM summaries (e.g., links to raw data)
- Use retrieval-augmented generation with curated intelligence sources
- Integrate review checkpoints in SOC or CTI workflows
- Redact sensitive internal identifiers before input to LLM

## 🔐 Security Considerations
- Enforce strict segmentation of internal vs. external threat sources
- Log and archive all LLM-generated summaries for post-incident review
- Ensure that summaries are flagged if based on unverified or low-confidence intel

---

> **Last Updated:** May 2025
