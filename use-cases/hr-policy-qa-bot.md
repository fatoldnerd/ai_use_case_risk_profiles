# Use Case: HR Policy Q&A Bot

## 📌 Business Description
Human Resources teams deploy LLM-powered bots to answer employee questions about company policies, benefits, onboarding, leave processes, and workplace guidelines. This reduces repetitive HR inquiries and enhances employee self-service.

## ⚙️ LLM Functionality
- Question answering
- Policy summarization
- Document parsing
- Multilingual support

## 🔍 Risk Mapping
| Risk Category             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Hallucination            | LLM may return incorrect or outdated policy info                           |
| Prompt Injection         | Malicious inputs may yield unintended answers                              |
| Sensitive Info Disclosure| Private HR data or internal-only policies may be exposed                   |
| Insecure Retrieval       | Unvetted or misclassified documents may be included in responses           |

## 🧩 Framework Alignment
### NIST AI RMF
- **Map:** Identify user roles and scope of accessible HR content
- **Measure:** Monitor accuracy and appropriateness of responses
- **Manage:** Enforce content access restrictions and fallback to HR personnel
- **Govern:** Define update protocols and HR ownership of LLM knowledge base

### OWASP LLM Risks
- LLM01: Prompt Injection  
- LLM02: Insecure Output Handling  
- LLM06: Sensitive Information Disclosure  
- LLM09: Overreliance

## 🛡 Mitigation Strategies
- Fine-tune with validated HR-approved policy documents
- Implement role-based access and redaction for sensitive policy clauses
- Use human fallback for complex or sensitive queries
- Version control the knowledge base and automate content refresh cycles

## 🔐 Security Considerations
- Restrict access to policy tiers by employee role
- Audit and log all user interactions for compliance
- Ensure sensitive HR topics are flagged and routed to humans when needed

---

> **Last Updated:** May 2025
