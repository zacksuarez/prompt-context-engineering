# Prompt & Context Engineering for FP&A

> A hands-on demonstration of how prompt engineering, context engineering, business rules, evidence constraints, and validation improve AI-generated financial analysis.

## 🎯 Purpose

This project explores how a basic AI prompt can be progressively improved into a reusable business-analysis template.

The use case is deliberately simple:

> Analyze a software expense variance for monthly FP&A reporting.

The goal is not just to generate better wording.

The goal is to design an AI instruction set that:

- uses the right business context
- applies explicit rules
- separates facts from assumptions
- avoids unsupported root-cause claims
- produces CFO-ready output
- validates its own calculations

---

# 📊 Example Data

| Metric | Value |
|---|---:|
| Actual | $625,000 |
| Forecast | $500,000 |
| Prior Year | $450,000 |

Calculated variances:

- Actual vs Forecast: **+$125,000 / +25.0%**
- Actual vs Prior Year: **+$175,000 / +38.9%**

---

# V1 — Basic Prompt

```text
Analyze the software expense variance and provide management commentary.
