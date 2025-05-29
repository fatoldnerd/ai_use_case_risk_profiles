# Use Case: Compliance Report Assistant

## 📌 Business Description
Regulatory, legal, and audit teams use LLMs to assist in compiling compliance reports, summarizing control evidence, and responding to auditor queries. The LLM helps streamline reporting cycles and supports alignment with frameworks like SOC 2, ISO 27001, or GDPR.

## ⚙️ LLM Functionality
- Document summarization
- Policy and control mapping
- Audit response drafting
- Language normalization

## 🔍 Risk Mapping
| Risk Category             | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| Hallucination            | LLM may generate inaccurate or misleading compliance claims                 |
| Sensitive Info Leakage   | Regulatory data or audit findings may be exposed to unauthorized users      |
| Insecure Output Handling | Generated text may misrepresent official positions or obligations           |
| Overreliance             | Teams may defer critical oversight to LLM-generated narratives              |

## 🧩 Framework Alignment
### NIST AI RMF
- **Map:** Identify the regulatory reporting workflows supported by the LLM
- **Measure:** Evaluate output fidelity, clarity, and completeness across frameworks
- **Manage:** Embed legal review and human sign-off into reporting pipelines
- **Govern:** Maintain change logs, version control, and escalation procedures

### OWASP LLM Risks
- LLM02: Insecure Output Handling  
- LLM05: Improper Output Handling  
- LLM06: Sensitive Information Disclosure  
- LLM09: Overreliance

## 🛡 Mitigation Strategies
- Implement predefined prompts based on control frameworks
- Use version-controlled templates and human-validated source data
- Require legal or GRC review of all generated content
- Mask sensitive audit findings from training prompts

## 🔐 Security Considerations
- Apply role-based access to compliance artifacts
- Store and encrypt draft and final reports securely
- Maintain audit trails for all LLM-generated contributions

---

> **Last Updated:** May 2025
