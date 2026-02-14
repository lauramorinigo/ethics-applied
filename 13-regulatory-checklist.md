This checklist is designed for inclusion in the **Project Appendix**. It allows auditors, compliance officers, and engineering leads to verify the legal alignment of the AI system at a glance.

---

## ## Appendix: Regulatory Compliance Checklist (Legal Alignment)

### ### Phase 1: Risk Classification & Mapping

* [ ] **Tier Assignment:** Has a **Total Risk Score (TRS)** been calculated using the Systematic Assessment Methodology (Domain, Autonomy, Scale, etc.)?
* [ ] **Annex III Verification:** For admissions/recruitment, has the system been officially logged as **"High-Risk"** in the organizational registry?
* [ ] **Jurisdictional Mapping:** Are requirements mapped for all active markets (e.g., EU AI Act, GDPR, US State Laws, Canada AIDA)?

### ### Phase 2: Technical Translation & Development

* [ ] **DoD Integration:** Does the **Definition of Done** for every fairness-related User Story include a link to automated test results?
* [ ] **Metric Alignment:** Are technical fairness metrics (e.g., Disparate Impact) linked to specific legal mandates (e.g.,  to  ratio for US/EU compliance)?
* [ ] **CI/CD Fairness Hooks:** Are `Fairlearn` or `AIF360` checks integrated into the build pipeline to prevent "Bias Regression"?

### ### Phase 3: EU-Specific Obligations (High-Risk)

* [ ] **Technical File (Annex IV):** Is there a comprehensive file detailing system logic, data provenance, and resource tracking?
* [ ] **Human-in-the-Loop (Art. 14):** Does the UI include a functional **"Override" or "Kill Switch"** for human reviewers?
* [ ] **Instruction for Use (Art. 13):** Is there a user-facing document explaining system accuracy, limitations, and the role of AI in the decision?
* [ ] **Logging (Art. 12):** Are automated decision logs being stored in an immutable, secure environment for traceability?

### ### Phase 4: Data Subject Rights (GDPR Art. 22)

* [ ] **Explanation Mechanism:** Can the system generate a "Meaningful Explanation" of logic (e.g., SHAP/LIME values) for rejected candidates?
* [ ] **Contestability Pathway:** Is there a documented URL or process for a candidate to request a **manual human review**?
* [ ] **Disclosure:** Are users informed *before* processing that they are subject to automated decision-making?

### ### Phase 5: Evidence & Audit Readiness

* [ ] **Automated Model Cards:** Is a JSON/Markdown Model Card generated automatically for every production-ready model version?
* [ ] **Intersectionality Audit:** Does the evidence bundle include performance data for compound groups (e.g., **Age + Race**)?
* [ ] **Retention Compliance:** Is the evidence bundle scheduled for a **10-year retention** period?
* [ ] **Red-Team Report:** Is there a documented "Safety Stress Test" report showing attempts to elicit biased or harmful outputs?

