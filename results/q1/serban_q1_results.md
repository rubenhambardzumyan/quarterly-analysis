# WS Engineering Q1'26 Plan - BrainLift Analysis

*Context: This is an Engineering manager's Q1 plan. BrainLifts will be built by Engineers, so expertise gaps should be relevant to engineering work.*

---

## TimeBack

### 1EdTech Platform

**Suggested BrainLift: "1EdTech Standards Implementation Principles"**

**Purpose Statement:**

*Problem:* The platform is making a significant technology bet on 1EdTech standards (LTI, OneRoster, CASE, Caliper, QTI) as the foundation for interoperability at scale. Engineers are implementing these standards but support is "partial"—LTI doesn't support deep linking or SSO scenarios, QTI storage needs more content types, Caliper events need extension.

*Expertise Gap:* Engineers are learning these standards as they implement them. Each standard has nuances that determine whether integrations work reliably at scale. Q1 includes extending Caliper, enhancing QTI, revamping LTI, continuing CASE modeling, and starting SDK development—all requiring deep understanding of these specifications.

*In Scope:*
- LTI implementation patterns for deep linking and SSO scenarios
- CASE curriculum modeling structures that support learning algorithms
- Caliper event design patterns for educational analytics
- QTI content storage architecture for flexibility and performance
- SDK design principles for third-party developer experience

*Out of Scope:*
- Business decisions about which standards to adopt
- Vendor partnerships
- Content creation

---

### Data Collection & Analytics

**No BrainLift needed.** Consolidating data from ~6 apps, refining WasteMeter to 95% precision, stabilizing clients, and exposing analytics views is engineering execution on known patterns.

---

### Outcome-Based Funding

**No BrainLift needed.** Computing payouts from XP + assessments and building funding-ready views is execution. The data model is defined.

---

### Outcomes Copilot

**No BrainLift needed.** Building a copilot product with defined requirements (answer diagnostic questions in ≤10 minutes) is engineering execution.

---

### Mastery & Assessments

**No BrainLift needed.** Integrating MasteryTrack/AlphaTest, capturing standardized tests, and prototyping VLH is integration and measurement work.

---

### Vault & Security

**No BrainLift needed.** Decoupling PII, implementing role-based access, audit logs, and security documentation follows established security engineering patterns.

---

## Alpha Enrollment & Administration

### Unified Data Platform

**No BrainLift needed.** Building a unified data model, workflow engine, and API is standard engineering work with clear requirements.

---

### Marketing & Communities

**No BrainLift needed.** Building AlphaCommunities and AlphaToMyCity platforms is product engineering with defined features.

---

### Admissions & Enrollment

**No BrainLift needed.** Building Parent Portal and Admissions Portal with workflow controls is execution.

---

### Tuition & Payments

**No BrainLift needed.** DocuSign-to-Stripe integration and payment dashboards is known integration work.

---

### School Operations (SIS)

**Clarifying question:** The document mentions "Buy vs build evaluation." Is this a decision where engineers need to develop expertise in evaluating SIS vendors against Alpha's specific requirements? Or is this a business decision that doesn't require engineering expertise development?

---

## Content Generation

### Simon's Incept - Content Generation

**No BrainLift needed.** Completing supplemental courses and migrating off CoachBot is production and engineering execution.

---

### Simon's Incept - Curriculum Design & Academic Validation

**Suggested BrainLift: "Pedagogical Rules for AI Content Generation"**

**Purpose Statement:**

*Problem:* AI-generated educational content fails without pedagogical expertise encoded into the generation pipeline. Engineers build and maintain the content generation system, but the rules that make content academically sound live in one SME's head. When content fails academic review, engineers need to understand why to fix the generation logic.

*Expertise Gap:* The document explicitly states the need to "document curriculum design decisions and pedagogical rules as reusable IP" and "build validation frameworks that catch common errors before human review." Engineers need these rules encoded so they can build automated validation and improve generation without bottlenecking on SME review.

*In Scope:*
- Pedagogical rules engineers can encode into generation prompts and validation
- Common error patterns and how to detect them programmatically
- Curriculum sequencing principles for automated content ordering
- Question type selection logic based on learning objectives

*Out of Scope:*
- Actual academic content review (that's SME work)
- Hiring additional SMEs
- Grade-level specific content decisions

---

### Shawn's Incept - Agentic Incept

**Suggested BrainLift: "Agentic Content Generation Architecture"**

**Purpose Statement:**

*Problem:* The team is moving from prototype to production-grade agentic content generation—a significant technology investment. This involves RAG-based curriculum standards search, Surfboard model flexibility (mixing models per task), tools for images/curriculum lookup/figures/animations, and multi-region tenancy. These architectural decisions will determine whether the system scales.

*Expertise Gap:* The document states the system is "currently at prototype/PoC stage. Not yet validated as production-grade architecture and infrastructure." Engineers need to develop principles for agentic AI system architecture: when to use tools vs. LLM reasoning, how to structure RAG for curriculum search, how to orchestrate multi-model pipelines, how to load-balance agentic workflows.

*In Scope:*
- Agentic architecture patterns for educational content generation
- RAG design principles for curriculum standards search
- Multi-model orchestration (Surfboard flexibility) patterns
- Tool design principles that reduce LLM cognitive load
- Production-grade scaling for agentic systems

*Out of Scope:*
- Educational principles (Direct Instruction, DOK) - that's curriculum expertise
- Specific curriculum content
- Business decisions about which curricula to support

---

### Shawn's Incept - InceptBench

**No BrainLift needed.** Building evaluation pipelines, expanding curriculum compatibility, and publishing benchmarks is engineering execution with clear goals.

---

## Learning Apps

### Athena

**No BrainLift needed.** CoachBot separation, LTI compliance, and MVP Course Builder are execution tasks with clear requirements.

---

### TeachTales

**No BrainLift needed.** Fixing issues from student sessions and implementing vocabulary teaching approach (once learning science input arrives) is engineering execution.

---

### GameDev (TrashCat)

**No BrainLift needed.** Building another game on the reusable fluency core and deeper TimeBack integration is engineering execution. The learning science input comes from Andy M.—engineers implement his specs.

---

### QTI Renderer

**No BrainLift needed.** Stabilizing and expanding a shared rendering component is infrastructure engineering with clear scope.

---

## Academic Outcome Validation

**No BrainLift needed.** Building a standardized validation framework is engineering execution. The methodology for validating learning outcomes is a research/academic question, not an engineering expertise gap.

---

## Legacy CoachBot

**No BrainLift needed.** Maintenance mode.

---

## Crossover

### Hiring Efficiency

**No BrainLift needed.** Improving BFQ completion rates and positioning Crossover for edtech jobs is product/marketing work, not engineering expertise.

---

### Filtering Quality - Video Submission Grading

**Clarifying question:** The document mentions "unclear rubrics" for video submission grading. Is this an engineering problem (how to build AI grading systems) or a hiring/assessment design problem (what criteria to evaluate)? If engineers need to build video grading AI but lack clear rubrics to train against, the rubric definition is a prerequisite—but it's likely not an *engineering* BrainLift.

---

### Filtering Quality - Domain-Specific Assessments

**Suggested BrainLift: "AI Assessment Design Patterns"**

**Purpose Statement:**

*Problem:* Q1 focus includes "Domain-specific AI assessments: scenario-based for support, simulation-based assessments." Engineers are building AI-graded assessments for multiple domains, but each new assessment type requires figuring out how to structure it, how to grade it with AI, and how to ensure fraud resistance.

*Expertise Gap:* The team is investing in new assessment technologies (simulation-based, scenario-based) beyond simple question-answer formats. This is a technology investment that requires developing principles for how to architect assessable simulations, how to design scenario-based assessments that AI can evaluate, and how to build fraud-resistant assessment systems.

*In Scope:*
- Architecture patterns for simulation-based assessments
- Scenario-based assessment design that enables AI grading
- Fraud detection and prevention patterns for AI assessments
- Plagiarism detection for AI-generated submissions

*Out of Scope:*
- What skills to assess (that's hiring/domain expertise)
- Rubric content (that's assessment design)
- Candidate evaluation decisions

---

### AI Automation

**No BrainLift needed.** Continuing coding practices into AIPIs and exposing to customers is execution on established patterns.

---

### Retention

**No BrainLift needed.** Filtering for culture fit and self-sufficiency is a hiring/HR problem, not an engineering expertise gap. "Establish quality bar for training materials" and "AI bot for team-specific ramp-up" are execution items.

---

## BrainLift Coach

**No BrainLift needed.** This initiative is about BrainLifting methodology and training—which is meta/organizational, not engineering work. Engineers on this team would build the product features (graduation exams, score reports, skill-building programs), not develop the BrainLifting methodology itself. The methodology expertise sits with the TPO/product owner.

---

## WorkSmart Coach

**Clarifying question:** Q1 focus is "TBD." Without defined direction, can't assess engineering expertise gaps.

---

## ProductMind

**No BrainLift needed.** Automating ModelFit, building proactive deal nudges, and VDR Analysis Agent are engineering execution with clear requirements. The M&A domain knowledge comes from the business team.

---

## TSI

**Clarifying question:** Problem and Vision are "Unclear," yet Q1 focus is "AI agent for customer outreach." What problem does this agent solve? Engineers need clear requirements before they can identify expertise gaps.

---

## Central Function

### Execute Strategic Initiatives

**No BrainLift needed.** Resource allocation, not expertise development.

---

### Launch $70/h Product Engineer Role

**No BrainLift needed.** Role definition and hiring pipeline is HR/org work.

---

### Revamp UI/UX Design to AI-First Workflow

**Suggested BrainLift: "AI-First UI Prototyping Workflow"**

**Purpose Statement:**

*Problem:* The document describes replacing the current designer with someone who does "AI-first prototyping (tools like Lovable for coded UIs, not wireframes)" and references "Abhinav's approach - rapid AI prototypes, test with users, iterate." This is a workflow shift that affects how engineers collaborate with design.

*Expertise Gap:* If engineers are expected to work with AI-generated coded UIs instead of wireframes, they need to understand this workflow. What tools produce what output? How do you iterate on AI-generated code? What's the handoff process? This is a technology investment in a new way of working that engineers will need to adopt.

*In Scope:*
- AI prototyping tools (Lovable, etc.) and their output formats
- Workflow patterns for iterating on AI-generated UI code
- Integration patterns between AI-generated prototypes and production codebases
- Quality standards for AI-generated UI code

*Out of Scope:*
- Design principles and aesthetics (that's design expertise)
- User research methodology
- Hiring decisions

---

## Summary

| Initiative | Outcome |
|------------|---------|
| **TimeBack - 1EdTech Platform** | **BrainLift: "1EdTech Standards Implementation Principles"** |
| TimeBack - Other modules | No BrainLift - Execution |
| Alpha E&A - SIS | Question: Is SIS vendor evaluation an engineering expertise gap? |
| Alpha E&A - Other modules | No BrainLift - Execution |
| **Simon's Incept - Curriculum Design** | **BrainLift: "Pedagogical Rules for AI Content Generation"** |
| **Shawn's Incept - Agentic Incept** | **BrainLift: "Agentic Content Generation Architecture"** |
| Learning Apps (all) | No BrainLift - Execution |
| Crossover - Video Grading | Question: Engineering problem or assessment design problem? |
| **Crossover - Domain-Specific Assessments** | **BrainLift: "AI Assessment Design Patterns"** |
| Crossover - Retention | No BrainLift - HR/hiring problem |
| BrainLift Coach | No BrainLift - Methodology is TPO/product work |
| WorkSmart Coach | Question: What is the Q1 direction? |
| ProductMind | No BrainLift - Execution |
| TSI | Question: What problem does the AI agent solve? |
| **Central Function - AI-First Design** | **BrainLift: "AI-First UI Prototyping Workflow"** |
