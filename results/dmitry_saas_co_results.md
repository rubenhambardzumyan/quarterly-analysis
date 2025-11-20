# Quarterly Plan Analysis: Dmitry SaaS VP of CO Q4

## Goal 1: Execute $3.1M PA CR for Khoros

**Identified Goal:** Deliver $3.1M per annum cost reduction via 3 kanbans ($1M each), planned by David S., with zero CO-related production outages and SLA adherence on CO tickets.

**Analysis:** This goal describes executing a pre-defined plan with clear targets, kanban allocation, and success metrics (SLA adherence, zero outages). The plan is already created by David S. No explicit evidence of lacking knowledge or capability to execute.

**Assessment:** This is execution of an existing plan, not an expertise gap.

---

## Goal 2: Execute $500k PA CR for Rest of ESW

**Identified Goal:** Deliver $500k per annum cost reduction for ESW portfolio using 1 kanban slot, seeded with "high-quality hypotheses actionable within the quarter."

**Analysis:** The goal mentions generating "high-quality hypotheses actionable within the quarter" and tracking "hypothesis → actionability conversion." The document provides a budget table showing accounts with significant variance from trailing 4Q average (ranging from 22% to 185%), marked as "primary targets for investigation."

However, there's no explicit statement about:
- What makes a hypothesis "high-quality" vs low-quality
- What determines "actionability within the quarter"
- Whether they lack the expertise to evaluate these, or simply haven't done the analysis yet

**Questions to Clarify:**
1. What expertise or decision framework is needed to turn budget variance data (22% to 185% deviations) into "high-quality hypotheses actionable within the quarter"? Is this judgment based on experience that needs to be formalized, or is it straightforward analysis?
2. What distinguishes quarterly-actionable cost reduction opportunities from multi-quarter efforts? Is this tacit knowledge that needs to be captured, or a known process?

**Assessment:** Insufficient evidence to determine if this is an expertise gap or execution. Need clarification on whether hypothesis generation requires formalizing tacit knowledge or is simply analytical work.

---

## Goal 3: Build AI-Driven Cost Anomaly Analysis Process

**Identified Goal:** Create automated pipeline that receives AWS Cost Anomaly alerts, enriches them with Cost Explorer/CloudWatch data, generates reports automatically delivered to account owners, and excludes "known noise" from reporting.

**Analysis:** The supporting data (DOK1/2) provides detailed descriptions of noise patterns:
- S3 storage tier transitions at month boundaries (need >10% threshold)
- CloudWatch custom metric tier switches ($0.30 → $0.10)
- EBS pricing variations in shorter months
- Weekly vs daily cost comparison patterns
- Tiered cost structures

This detailed documentation suggests they already understand these patterns and know what constitutes "noise." The goal is to automate the application of this knowledge.

No explicit evidence that they lack the expertise to classify anomalies or set thresholds—the supporting data demonstrates they already possess this knowledge.

**Assessment:** This is execution/automation of known patterns, not an expertise gap. They're building infrastructure to apply existing knowledge automatically.

---

## Goal 4: Build AI Runbooks for Health Checks After CO Changes

**Identified Goal:** Create automated runbooks covering at least 60% of CO tickets, with automated metadata collection and runbook output published as GitHub comments.

**Analysis:** The document describes the automation mechanics (GitHub metadata extraction, AWS ReadOnly IAM role, automatic publishing) but doesn't explain:
- What determines runbook quality or comprehensiveness
- Why 60% coverage is the target (vs higher or lower)
- What makes certain CO changes suitable for automated runbooks vs requiring manual validation
- What the risk tolerance is for automated validation

No explicit evidence of an expertise gap. The goal appears to be building automation infrastructure.

**Questions to Clarify:**
1. What determines when an automated runbook is "good enough" to validate a CO change vs when human verification is required? Is this decision based on formalized risk criteria or tacit judgment?
2. Why is 60% the coverage target? What characterizes the 40% that won't be automated?

**Assessment:** This appears to be execution/feature development, but need clarification on the decision framework for runbook scope and risk tolerance.

---

## Goal 5: Streamline Cost Reporting

**Identified Goal:** Create a spec that documents decisions around amortization and cost tracking, then implement a script that automatically produces weekly budget reports.

### Sub-goal 5.1: Document Amortization Decision Framework

**Analysis:** The goal states "There is a Spec that documents decisions around..." which indicates the spec needs to be created. The supporting data (DOK1/2) describes complex amortization challenges in detail:

**Time-Based Amortization:**
- Marketplace contracts and reservations spread over 1-3 years (otherwise "distort the lookback window—spiking spend when they hit, and lowballing it when they don't")
- Monthly backup storage charges spread across all days
- Monthly EBS volume pricing adjusted for shorter months

**Account-Based Amortization:**
- Support fees, unused Savings Plans, and cRIs spread proportionally across accounts

**Cost Anomaly Thresholds:**
- S3 storage: >10% threshold to avoid false alarms from tier transitions
- CloudWatch: ignore MetricMonitorUsage spikes from tier changes
- Weekly vs daily comparison for weekly product cycles

**Critical Question:** Does this detailed documentation in the supporting data represent:
1. **Existing decisions that need to be written down** (execution—documenting known rules), OR
2. **Tacit knowledge that needs to be formalized into a decision framework** (expertise gap—turning experience into reusable process)?

The document states these rules are needed because without them, reports "distort the lookback window" and "trigger avoidable back-and-forth with BUs," suggesting the decisions exist but aren't formally documented.

**Questions to Clarify:**
1. Are the amortization rules and anomaly thresholds described in DOK1/2 already established practices that need to be documented, or are they expertise that needs to be developed and formalized?
2. If these are established practices, what's preventing them from being documented now? If they're not established, what's the expertise gap?

**Assessment:** Could be either expertise gap (formalizing tacit knowledge about amortization decisions) OR execution (documenting existing rules). Need clarification on whether the knowledge exists and needs documentation vs needs to be developed.

---

### Sub-goal 5.2: Implement Automated Reporting Script

**Analysis:** Once the spec exists, implementing a script to automate weekly report generation is technical execution.

**Assessment:** This is execution, not an expertise gap.

---

## Summary of Recommendations

**No BrainLifts Proposed** - Insufficient explicit evidence of expertise gaps in the document.

**Execution/Operations Items (3):**
- Goal 1: Execute Khoros cost reduction plan
- Goal 3: Build cost anomaly automation pipeline
- Goal 5.2: Implement reporting script

**Goals Requiring Clarification (3):**

**Goal 2 (ESW Cost Reduction Hypotheses):**
- What expertise is needed to generate "high-quality hypotheses actionable within the quarter"?
- Is hypothesis generation based on tacit knowledge that needs formalization, or is it straightforward analysis?

**Goal 4 (AI Runbooks):**
- What determines when automated runbooks are sufficient vs requiring manual validation?
- Why 60% coverage? What characterizes the remaining 40%?

**Goal 5.1 (Cost Reporting Spec):**
- Are the amortization rules and anomaly thresholds in DOK1/2 existing practices needing documentation, or expertise needing development?
- If documenting existing practices, what blocks this now? If developing expertise, what's the gap?
