# Use Case: Customer Sentiment Analyzer

## 📌 Business Description
Customer experience and product teams use LLMs to analyze sentiment in support tickets, survey responses, and social media mentions. The goal is to detect dissatisfaction trends, prioritize product fixes, and track brand perception.

## ⚙️ LLM Functionality
- Sentiment classification
- Topic clustering
- Emotion tagging
- Trend summarization

## 🔍 Risk Mapping
| Risk Category             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Hallucination            | LLM may misclassify sentiment, leading to misprioritization                |
| Overreliance             | Decisions may be made without verifying context or source nuance           |
| Insecure Output Handling | LLM-generated summaries may exaggerate or dilute important feedback        |
| Sensitive Info Disclosure| Individual customer feedback may be surfaced improperly in summaries       |

## 🧩 Framework Alignment
### NIST AI RMF
- **Map:** Define the types of customer inputs analyzed and the stakeholders using results
- **Measure:** Track false positive/negative rates in sentiment classification
- **Manage:** Layer human validation for flagged issues or automated reports
- **Govern:** Audit sentiment scoring logic and reporting workflows

### OWASP LLM Risks
- LLM02: Insecure Output Handling  
- LLM05: Improper Output Handling  
- LLM06: Sensitive Information Disclosure  
- LLM09: Overreliance

## 🛡 Mitigation Strategies
- Include confidence scores and explanation layers with sentiment outputs
- Filter or anonymize personally identifiable content before analysis
- Require manual review before escalation or public response
- Version and trace sentiment outputs used in strategy decisions

## 🔐 Security Considerations
- Enforce data masking on direct customer quotes
- Apply access control to raw input and summary outputs
- Log usage and changes to LLM sentiment processing models

---

> **Last Updated:** May 2025
