# SaaS VP of CO Problems Decomposition

### Intro

The goal of this document is to break down the Q4/2025 plan of SaaS VP of CO (Cost Optimization) into problems to analyze BrainLift opportunities for each problem and present either a purpose statement or questions to clarify before a BrainLift with a purpose statement can be presented.

### Thought Process

- **The Priority**
  - Identify good goals, and use those good goals to articulate a good purpose statement in cases a BrainLift can be suggested
  - Using questions to understand the goals deeper and improve the goals, thus being able to suggest a BrainLift with a good purpose statement
- **Goal Extraction & Validation**
  - Extract all stated goals from the document
  - For each goal, assess whether it is actionable as-is or requires decomposition:
    - Can specific problems or decisions be identified from the document context?
    - Is the goal describing a problem to solve, or merely a desired outcome?
    - Does the document provide sufficient context about current state, challenges, or approach?
    - Are there enough context and understanding to decompose it into complete, actionable work sub goals?
- **Problem Identification**
  - Extract underlying problems from:
    - Explicit problem statements in the document.
    - Challenges mentioned in context.
    - Gaps between current state and goal.
  - Avoid inventing problems not present in the document.
- **Problem Analysis**
  - For each identified problem, assess clarity:
    - If clearly defined:
      - Determine whether solving it requires developing expertise (not just executing tasks).
        - If expertise development is needed, then propose a BrainLift with clear purpose statement and use the context to articulate a clear, high quality purpose. In case of gaps, list the curious questions that need to be answered and prepare to clarify them with the user
        - If execution only, then note that it is an execution task, not a BrainLift candidate.
    - If not clearly defined:
      - List specific curious questions needed to clarify:
        - What is the current state?
        - What are the actual challenges?
        - What has been tried?
        - What decisions need to be made?
        - What expertise is lacking?
- **Quality Standards**
  - Never propose a BrainLift without a clear, specific purpose statement.
  - If the purpose statement merely restates the goal, insufficient context exists.
  - When in doubt, ask clarifying questions rather than make assumptions

### **SaaS VP of CO Q4 Goals**

- **Goal 1 (as stated): Execute $3.1M PA CR for Khoros**

  - Target as specified in the document:
    - Deliver $3.1M PA cost reduction
    - Execute via 3 kanbans ($1M per kanban) as planned by David S.
    - All approved CO tickets executed in a timely manner
    - Zero CO-related production outages
    - SLA adherence on CO tickets
  - Identified problems:
    - Goal doesn't articulate what problem needs solving
      - No BrainLift to propose, since the document states targets and metrics but doesn't explain what makes this challenging or what expertise is needed. It mentions executing "via 3 kanbans ($1M per kanban) as planned by David S." suggesting the approach is already defined.
      - Questions to clarify:
        - On problem:
          - What specific challenges exist in executing the $3.1M cost reduction?
          - What decisions need to be made that aren't already defined in David S.'s plan?
          - What makes this different from straightforward execution of approved tickets?
        - On expertise needed:
          - What expertise or judgment is required beyond following the planned kanban approach?
          - What quality standards or decision criteria need to be developed?
          - What has made previous cost reduction efforts successful or unsuccessful?

- **Goal 2 (as stated): Execute $500k PA CR for Rest of ESW**

  - Target as specified in the document:
    - Deliver $500k PA cost reduction for ESW portfolio
    - Use 1 kanban slot for execution
    - Seed kanban with high-quality hypotheses actionable within the quarter
    - Zero CO-related production outages
    - Hypothesis to actionability conversion tracked
  - Identified problems:
    - Generating high-quality, actionable cost reduction hypotheses
      - No BrainLift to propose, since the document mentions needing "high-quality hypotheses actionable within the quarter" and shows a budget table with accounts and "DIFF TO AVG" percentages, with some accounts "highlighted in yellow" as "primary targets for investigation." However, it doesn't explain what makes hypotheses high-quality, what makes them actionable, what challenges exist in generating them, or how to interpret the budget variance data to create hypotheses.
      - Questions to clarify:
        - On problem:
          - What specific challenges exist in generating cost reduction hypotheses for ESW?
          - What makes a hypothesis "high-quality" vs low-quality?
          - What determines whether a hypothesis is "actionable within the quarter"?
        - On current state:
          - How are hypotheses currently generated and what's problematic about that process?
          - What percentage of generated hypotheses typically turn out to be actionable?
          - What has prevented achieving $500k cost reduction in previous quarters?
        - On the budget data:
          - How should the "DIFF TO AVG" percentages in the budget table inform hypothesis generation?
          - What criteria determine which accounts are "primary targets for investigation"?
          - Are accounts with high variance (e.g., 182.65%, 185.99%) always good targets, or are there other factors?

- **Goal 3 (as stated): Build AI-Driven Cost Anomaly Analysis Process**

  - Target as specified in the document:
    - Automatic pipeline receives AWS Cost Anomaly alerts
    - AI agent enriches anomalies with Cost Explorer/CloudWatch data
    - Report automatically generated and delivered to account owner & SaaS DRI
    - Known noise (usage tiers, amortization gaps) excluded from reporting
    - % anomalies successfully processed and delivered to account owners
    - % of anomalies remediated within the quarter
    - Cost savings $$ PA
  - Identified problems:
    - Distinguishing actionable cost anomalies from known noise patterns
      - Possible BrainLift: Cost anomaly classification and noise filtering framework
      - Purpose: The document states that "known noise (usage tiers, amortization gaps)" must be excluded from reporting, and the supporting data provides specific examples of noise patterns that require expert judgment: S3 storage costs that spike when usage rolls from $0.021/GB tier to $0.023/GB tier at month boundaries (requiring threshold above 10%), CloudWatch MetricMonitorUsage spikes from $0.30 tier before switching to $0.10 (requiring ignore rules), EBS volume pricing that appears higher per day in shorter months like February (requiring month-length adjustment), and distinguishing weekly cycle patterns from actual anomalies (comparing same day last week vs day before). The challenge is developing expertise in distinguishing real cost anomalies that require action from predictable noise patterns that will trigger false alarms and waste account owners' time. This requires establishing clear decision criteria for: when cost variations represent genuine issues vs expected behavior, what thresholds to set for different service types, and how to handle edge cases like tiered pricing transitions.
        - In scope:
          - Framework for classifying cost anomalies as actionable vs known noise
          - Threshold-setting methodology for different AWS service types (S3, CloudWatch, EBS)
          - Decision criteria for weekly vs daily cost comparison patterns
          - Edge case handling rules for tiered pricing transitions and month-length variations
        - Out of scope:
          - AI/ML implementation or technical architecture
          - AWS Cost Explorer or CloudWatch API integration details
          - Report formatting or delivery mechanisms
          - Account owner notification processes

- **Goal 4 (as stated): Build AI Runbooks for Health Checks After CO Changes**

  - Target as specified in the document:
    - Runbooks cover at least 60% of CO tickets
    - Automatically pull resource metadata (name, region, etc.) from GitHub issue
    - Use ReadOnly AWS IAM role to collect environment data
    - Automatically publish runbook output as a GitHub issue comment
    - Coverage % of CO tickets
    - % automation of metadata collection
  - Identified problems:
    - Target lacks context about what problems it solves
      - No BrainLift to propose, since the document describes the technical components (metadata extraction from GitHub, AWS data collection via ReadOnly IAM, automated comment publishing) but doesn't explain what makes this challenging beyond engineering implementation. The 60% coverage target is stated but without context about what determines which tickets can be covered, what quality standards the runbooks need to meet, or what problems current health check processes face.
      - Questions to clarify:
        - On problem:
          - What problems do health checks after CO changes currently face that AI runbooks would solve?
          - Why is 60% coverage the target rather than higher or lower?
          - What makes certain CO tickets suitable for runbooks vs not?
        - On expertise needed:
          - What determines if a runbook is "good enough" to replace manual health checks?
          - What trade-offs exist between runbook coverage and quality/accuracy?
          - What decisions need to be made about which checks to include in each runbook?
        - On current state:
          - How are health checks currently performed and what's problematic about that approach?
          - What percentage of current health checks could be automated with clear criteria vs require human judgment?
          - What happens when runbooks miss issues that manual checks would have caught?

- **Goal 5 (as stated): Streamline Cost Reporting**

  - Target as specified in the document:
    - Create a Spec documenting decisions around amortization of upfront reservations and AWS marketplace yearly contracts, separate tracking of AI, EY and Wine Cellar costs
    - Create a script that implements these decisions and automatically produces weekly reports
  - Identified problems:
    - Cost amortization and anomaly detection require expertise in handling complex edge cases
      - Possible BrainLift: Cost amortization and reporting decision framework for SaaS infrastructure
      - Purpose: The document states the need for "a Spec that documents decisions around amortization" and provides extensive supporting data about cost amortization and anomaly detection challenges that require expert judgment to avoid "distorting the lookback window" and "triggering avoidable back-and-forth with BUs." Time-based amortization must handle marketplace contracts and reservation upfront fees spread over 1-3 years (otherwise "spiking spend when they hit, and lowballing it when they don't" throws off forecasts), plus backup storage charges that hit on the 1st but should spread over the month. Account-based amortization must proportionally spread support fees and unused savings plans across accounts. Cost anomaly detection must handle tiered pricing (S3 storage threshold above 10% to avoid false alarms at month boundaries, CloudWatch metric tier transitions), monthly pricing variations (EBS costs higher in February), and weekly cycle patterns (comparing same day last week, not previous day). The expertise needed is developing clear decision rules for when and how to amortize different cost types, what thresholds to set for anomaly detection across different services, and how to handle edge cases while maintaining accurate reporting that stakeholders trust and use for forecasting.
        - In scope:
          - Decision framework for time-based amortization (reservations, marketplace contracts, monthly charges spread across days)
          - Rules for account-based amortization across proportional spend (support fees, unused savings plans)
          - Anomaly detection threshold methodology for different AWS services (S3, CloudWatch, EBS)
          - Edge case handling (tiered pricing transitions, monthly variations in shorter months, weekly cycle patterns)
        - Out of scope:
          - Script implementation or technical automation details
          - Report formatting or visualization design
          - AWS billing API integration
          - Stakeholder communication or BU coordination processes
