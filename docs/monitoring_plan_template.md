
# Monitoring Plan Template

## How to Use This Template

This document provides a structured format for monitoring fairness performance in regulated AI systems.
It is aligned with Article 61 of the EU AI Act and supports internal or external conformity documentation.

Each section includes:
- **Fields** to be completed with system-specific information
- **Tables** for recurring evaluation and response planning
- A **change log** for edit accountability

Add one row per monitored metric, trigger condition, or responsible party for each table.
Fields marked with “[e.g.]” are illustrative and should be replaced.

---

## 1. System Overview

- **System name**: [e.g., CreditScoringML-v2]
- **Version**: [e.g., 1.0.1]
- **Deployment context**: [e.g., Internal loan approvals for SME lending]
- **Last updated**: [YYYY-MM-DD]
- **Monitoring Plan Owner**: [Person accountable for ongoing monitoring and review]
- **Last Edited By**: [Person who last made changes to this document]

## 2. Monitored Metrics

| Metric Name       | Group(s) Monitored | Frequency | Threshold for Action | Rationale |
|-------------------|--------------------|-----------|----------------------|-----------|
| TPR (Recall)      | A, B               | Weekly    | Disparity > 5%       | Detects under-service for protected groups |
| FPR               | A, B               | Monthly   | Disparity > 3%       | Monitors potential over-policing of one group |

## 3. Data Sources

- **Evaluation dataset**: [e.g., sampled real-world production logs]
- **Logging mechanism**: [e.g., internal API instrumentation]
- **Bias auditing pipeline**: [e.g., Airflow DAG triggering every 24h]

## 4. Trigger Conditions and Escalation

Describe what happens if thresholds are breached.

- **Trigger definition**: [e.g., If disparity > 5% for 2+ weeks]
- **Escalation path**: [e.g., Notify ML team lead + ethics officer]

## 5. Responsible Parties

| Role                 | Name / Contact      |
|----------------------|---------------------|
| Monitoring Lead      |                     |
| Model Owner          |                     |
| Ethics / Compliance  |                     |
| Documentation Lead   |                     |

## 6. Review Schedule

- **Review frequency**: [e.g., Quarterly]
- **Next review date**: 
- **Update criteria**: [e.g., Significant retraining, regulation change]

## 7. Notes

[Add any additional context or considerations here.]

---

## 8. Change Log
Any changes to the document should be recorded and attributed to an individual. Ideally, the changes in the document should be version-controlled (e.g., using git or similar). An example of an entry is provided below.

| Date       | Edited By         | Change Summary                                 | Review Status |
|------------|-------------------|------------------------------------------------|----------------|
| 2024-04-18 | Aaron Ceross       | Created initial monitoring plan template       | Draft          |
