
# Trade-off Log Usage Guide

This guide explains how to complete the trade-off log template, which is used to document fairness–accuracy trade-offs in AI systems subject to regulatory oversight (e.g., the EU AI Act, ISO/IEC 42001).

The log supports internal justification, conformity documentation, and reproducibility of mitigation decisions.

## Column Descriptions

- **Date**: When the trade-off decision or log entry was finalised (YYYY-MM-DD).
- **Model Version**: Version identifier (e.g., v1.2.0) of the system affected.
- **Mitigation Strategy**: The bias mitigation applied (e.g., thresholding, reweighting, exclusion).
- **Fairness Metric(s)**: Metrics used to evaluate disparity (e.g., TPR, FPR, AUC, calibration).
- **Group(s) Affected**: Groups involved in disparity analysis (e.g., Group A, Group B, gender, ethnicity).
- **Performance Before Mitigation**: Group-specific values before mitigation (can be a text string or dictionary-style).
- **Performance After Mitigation**: Same format as above, post-intervention.
- **Justification Summary**: Plain-language rationale for accepting the trade-off (referencing impact assessments, policy constraints, stakeholder feedback, or legal obligations).
- **Residual Risk**: Any introduced or remaining risks to fairness, accuracy, or compliance.
- **Alternative Strategies Considered**: What else was tested or ruled out and why.
- **Monitoring Plan Reference**: Name of the linked monitoring file or ID for tracking.
- **Approval / Reviewer**: Name of person or role who reviewed or authorised the mitigation decision.

## Best Practices

- Be specific. Avoid vague summaries like “improved fairness.”
- Use numbers when possible (e.g., “TPR increased from 0.62 to 0.71”).
- Link each entry to documentation, version history, and monitoring plans.
- Update the log when changes are made; treat it as a living artefact.
- Ensure reviewer or approver roles are assigned for audit purposes.

## Example

See the file: `tradeoff_log_annotated_example.csv` for a completed entry.

