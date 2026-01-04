# agents.md
## Business Acquisition Dashboard – Execution Rules

---

## 1. Core Objective
This application exists to evaluate the health, risk, and financeability of an existing small business acquisition using standardized inputs and repeatable decision logic.

The tool must:
- Reduce emotional bias
- Surface hidden risk
- Standardize deal evaluation
- Be usable by both first-time and experienced buyers

---

## 2. Data Philosophy
- All inputs are assumed imperfect
- No metric is trusted without context
- Missing data must be handled explicitly
- Assumptions must always be visible

---

## 3. Supported Input Types
Priority order:
1. CSV (preferred)
2. Excel (.xlsx)
3. PDF (parsed + reviewed)

PDF-derived data must be clearly labeled as “extracted” and require user confirmation.

---

## 4. Canonical Financial Model
Internally normalize all deals to:
- Revenue
- Cost of Goods Sold
- Gross Profit
- Operating Expenses
- EBITDA
- SDE (if applicable)
- Owner Add-Backs
- Working Capital Metrics

All downstream analysis must reference this normalized structure.

---

## 5. Scoring Rules
- Every score must be explainable
- No black-box models
- Scores are directional, not absolute
- Red flags override numeric scores

---

## 6. Deal Evaluation Principle
A deal that only works under optimistic assumptions is automatically flagged as high risk.

---

## 7. Non-Goals
This application does NOT:
- Replace legal diligence
- Replace Quality of Earnings
- Predict future performance with certainty
- Automate deal approval

It supports judgment; it does not replace it.

---

## 8. Modularity Requirement
Each tab must function independently:
- Analysis
- Comparison
- Financing
- Scorecard
- LOI
- Dashboard

Failure in one module must not break the application.

---

## 9. Security & Sharing
Authentication is optional during early development.
The architecture must support:
- Read-only sharing
- Per-deal isolation
- Future multi-user access

---

## 10. Design Rule
Clarity beats cleverness.
