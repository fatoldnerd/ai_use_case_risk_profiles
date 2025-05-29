# Use Case: RFP Response Builder

## 📌 Business Description
Sales and pre-sales teams use LLMs to draft and refine responses to Requests for Proposals (RFPs), Security Questionnaires, and Due Diligence forms. The LLM helps accelerate the response process by referencing a curated knowledge base of prior submissions and internal documentation.

## ⚙️ LLM Functionality
- Contextual Q&A
- Text generation and completion
- Retrieval of past answers
- Formatting and summarization

## 🔍 Risk Mapping
| Risk Category             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Hallucination            | LLM may fabricate compliance claims or certifications                      |
| Sensitive Info Leakage   | Prior confidential customer data may be reused or exposed                  |
| Insecure Output Handling | Generated answers may not align with current product capabilities          |
| Prompt Injection         | Maliciously crafted questions may extract unintended information           |

## 🧩 Framework Alignment
### NIST AI RMF
- **Map:** Define where in the sales cycle the LLM is used (e.g., proposal drafting, legal review)
- **Measure:** Track hallucination rate and legal/compliance deviations in outputs
- **Manage:** Limit LLM access to vetted, version-controlled documents
- **Govern:** Review usage policy, versioning controls, and cross-functional approval flows

### OWASP LLM Risks
- LLM01: Prompt Injection  
- LLM02: Insecure Output Handling  
- LLM06: Sensitive Information Disclosure  
- LLM09: Overreliance

## 🛡 Mitigation Strategies
- Implement retrieval-augmented generation (RAG) based on validated knowledge base
- Use approval workflows requiring human validation for compliance or legal assertions
- Redact sensitive deal-specific information from training or context files
- Enforce data segmentation by client or business unit

## 🔐 Security Considerations
- Apply strict access control to historical RFPs and documentation
- Monitor and log generated content used in external communications
- Ensure generated claims are reviewed by legal or compliance before submission

---

> **Last Updated:** May 2025
