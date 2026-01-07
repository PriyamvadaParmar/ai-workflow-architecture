# Input Schema

## Purpose
This document defines the **expected input structure** for the AI workflow.

By formalizing inputs, the workflow ensures consistency, repeatability, and predictable behavior across runs, datasets, and users.

The schema supports both **structured and unstructured inputs**, acknowledging real-world data constraints.

---

## Supported Input Types

### 1. Structured Data Inputs
Structured inputs may include tabular or semi-tabular data such as:

- Workforce headcount by period
- Attrition counts or rates
- Department or team identifiers
- Tenure bands
- Manager-to-employee ratios (if available)

#### Example Fields
```text
time_period
department_name
headcount
attrition_count
attrition_rate
tenure_band

Contextual metadata that provides interpretive support:


organization_size
industry_type
analysis_timeframe
geographic_scope


Unstructured Inputs


Unstructured inputs may include:
Qualitative notes from stakeholders
Observations from managers or analysts
Explanatory context about organizational changes


These inputs are preserved as context and must not be treated as evidence unless explicitly supported by structured data.


Input Quality Expectations


Inputs may be:
Incomplete
Inconsistent
Partially missing


The workflow is designed to detect and surface these conditions, not silently compensate for them.


Required vs Optional Inputs
Required

At least one structured workforce indicator (e.g., headcount or attrition)

Optional
Tenure distributions
Department metadata
Qualitative context


If required inputs are missing, the workflow must halt downstream reasoning and report insufficiency.
Validation Rules
Field names must be clearly labeled
Time periods must be explicitly defined
Units and percentages must be consistent or normalizable
Missing values must be preserved, not inferred


Pattern and Trend Finding 

detected_trends
concentration_patterns
anomalies
pattern_strength_classification
ambiguity_flags


Risk Diagnostics

risk_category
risk_severity
confidence_level
supporting_patterns
diagnostic_notes


Strategic Recommendations

recommendation
related_risk
priority_level
expected_impact
implementation_considerations
assumptions_and_limitations

Output Characteristics

All outputs must be:
Traceable to prior reasoning stages
Explicitly qualified by confidence levels
Free from unsupported causal claims
Suitable for non-technical decision-makers
Longitudinal Comparability


The schema is designed so that outputs from different runs can be:
Compared over time
Reviewed across business units
Audited after logic updates

