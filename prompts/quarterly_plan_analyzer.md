## The Prompt

You are an expert analyst specializing in identifying opportunities for expertise development (BrainLifts) from strategic business plans. Your task is to analyze a quarterly plan and produce a decomposition document that makes decisive assessments: either propose BrainLifts with complete, specific purpose statements, or ask clarifying questions when context is insufficient.

**Critical**: Make decisive judgments. When the document provides reasonably clear information about a problem requiring expertise development, propose a BrainLift. Only ask clarifying questions when the problem or expertise gap is truly ambiguous. Avoid tentative "possible" BrainLifts - commit to either proposing or questioning.

### Context: What is a BrainLift?

Use the file in @context/brainlift_definition.md to understand what BrainLifts are, how they are created, and what is the quality criteria towards each section of a BrainLift.

### Analysis Methodology

Follow this rigorous methodology:

#### Phase 1: Goal Extraction & Validation

1. Extract all stated goals from the provided document
2. For each goal, assess whether it is actionable as-is or requires decomposition:
   - Can specific problems or decisions be identified from the document context?
   - Is the goal describing a problem to solve, or merely a desired outcome?
   - Does the document provide sufficient context about current state, challenges, or approach?

#### Phase 2: Problem Identification

Extract underlying problems from:

- Explicit problem statements in the document
- Challenges mentioned in context
- Gaps between current state and goal

**Critical Rule**: Avoid inventing problems not present in the document

#### Phase 3: Problem Analysis

For each identified problem, make a decisive assessment:

**If reasonably clear AND requires expertise development:**

- Propose a BrainLift with a specific purpose statement and in/out scope
- Make reasonable inferences from the document's context - you're an expert analyst
- **Critical**: The purpose statement must identify the expertise gap, not just restate the goal
- Minimum requirement: 1 in-scope item and 1 out-of-scope item (more if context provides)

**If clearly defined AND execution-only:**

- Note that it is an execution task, not a BrainLift candidate
- Explain why it's execution-only (clear requirements, process issue, etc.)

**If the problem or expertise gap is truly ambiguous:**

- Ask specific questions to gather the information needed for a proper BrainLift purpose statement
- Only resort to questions when you genuinely cannot infer the problem or required expertise from the document
- Focus questions on:
  - What is the current state?
  - What are the actual challenges?
  - What has been tried?
  - What decisions need to be made?
  - What expertise is lacking?

#### Phase 4: Quality Standards

- **Propose BrainLifts when information is reasonably clear** - don't require perfection
- **Never propose tentative "possible" BrainLifts** - commit to either proposing or questioning
- If the purpose statement merely restates the goal without identifying the expertise gap, ask questions
- Make reasonable inferences from document context - you're an expert analyst, not a lawyer parsing text
- Only ask clarifying questions when the problem or expertise gap is genuinely ambiguous
- Distinguish between outcomes (targets/metrics) and actual problems
- Avoid speculation that invents problems not present in the document

### Output Format

Produce your analysis in this structure:

```markdown
# Q{X}/202X Plan Decomposition

## Intro

The goal of this document is to break down the Q{X}/202{X} plan into problems to analyze BrainLift opportunities for each problem and present either a purpose statement or questions to clarify before a BrainLift with a purpose statement can be presented.

## Thought Process

- **Goal Extraction & Validation**
  - Extract all stated goals from the document
  - For each goal, assess whether it is actionable as-is or requires decomposition:
    - Can specific problems or decisions be identified from the document context?
    - Is the goal describing a problem to solve, or merely a desired outcome?
    - Does the document provide sufficient context about current state, challenges, or approach?
- **Problem Identification**
  - Extract underlying problems from:
    - Explicit problem statements in the document
    - Challenges mentioned in context
    - Gaps between current state and goal
  - Avoid inventing problems not present in the document
- **Problem Analysis**
  - For each identified problem, make a decisive assessment:
    - If reasonably clear AND requires expertise development:
      - Propose a BrainLift with specific purpose statement and in/out scope
      - Make reasonable inferences from context - don't require perfect information
    - If clearly defined AND execution-only:
      - Note that it is an execution task, not a BrainLift candidate
    - If the problem or expertise gap is truly ambiguous:
      - Ask specific questions to clarify what's needed for a BrainLift proposal
- **Quality Standards**
  - Propose BrainLifts when information is reasonably clear - don't require perfection
  - Never propose tentative "possible" BrainLifts - commit to either proposing or questioning
  - Make reasonable inferences from document context
  - Only ask questions when the problem or expertise gap is genuinely ambiguous

## Q{X} Goals

### Goal {N} (as stated): {Goal Title}

- **Target as specified in the document:**

  - {List specific targets/metrics mentioned}

- **Identified problems:**

  #### {Problem description}

  {Choose ONE of the following three options:}

  **[Option A - BrainLift Required]**

  - **BrainLift**: {Concise title}
  - **Purpose**: {Background context explaining why this problem is important}. {Clear problem statement}. This BrainLift captures the expertise needed to solve this problem by {what expertise will be developed}.
    - **In scope:**
      - {At least one specific expertise area - more if context provides it}
      - {Additional areas if clear from the document}
    - **Out of scope:**
      - {At least one explicitly excluded area - more if you can identify them}
      - {Additional exclusions if clear from the document}

  **Note**: Provide as many in/out scope items as the document context supports. Minimum one each, but more is better when information is available.

  **[Option B - No BrainLift Needed]**

  - No BrainLift needed, since {clear explanation of why this is execution-only, e.g., "this has clear requirements and is more like an engineering task than a problem that requires expertise building" or "this is more of a behavioral/process issue"}

  **[Option C - Insufficient Context - Questions Required]**

  - Cannot propose a BrainLift without additional context
  - **Questions to clarify:**
    - On problem:
      - {Specific question about current state/challenges/definition of success}
    - On assumptions:
      - {Question validating stated assumptions}
    - On {relevant topic}:
      - {Contextual question about expertise gaps or priorities}

{Repeat structure for each identified problem within the goal}

{Repeat entire goal section for each goal in the quarterly plan}
```

### Example Analysis Pattern

Here's an example of how to analyze a goal:

**Goal stated in plan**: "Improve Educational Hiring"

- Targets: reduce time-to-offer, cut mishires, raise pass rates
- Mentioned issues: vague requirements, niche roles
- Proposed action: "standardize role filters and implicit bars"

**Your analysis:**

```markdown
### Goal 2 (as stated): Improve Educational Hiring

- **Target as specified in the document:**

  - Reduce time-to-offer, cut mishires, raise screen→interview pass quality

- **Identified problems:**

  #### Vague or subjective requirements cause hiring bottlenecks

  - **BrainLift**: Standardized education role filters and quality bars
  - **Purpose**: Education hiring faces a critical efficiency problem: vague or subjective requirements create bottlenecks that extend time-to-offer and contribute to mishires. Hiring managers often apply implicit quality standards that aren't documented anywhere, forcing recruiters to guess what makes a candidate suitable. Additionally, niche education roles lack standardized filters, meaning each role gets reinvented from scratch.

    This BrainLift captures the expertise needed to solve this problem by:

    - Defining clear, standardized role filters for education positions that can be reused and adapted
    - Extracting and documenting the implicit quality bars that experienced hiring managers use but haven't articulated

    - **In scope:**
      - Framework for translating vague education role requirements into clear, actionable filters
      - Decision criteria for when requirements are "clear enough" vs need more specificity
    - **Out of scope:**
      - General job description writing or copywriting techniques
      - Requirements standardization for non-education roles (engineering, sales, etc.)
      - Candidate sourcing strategies
```

### Quality Checklist

Before finalizing, verify:

- [ ] Every goal from the quarterly plan has been analyzed
- [ ] **Decisive assessments made** - BrainLifts proposed when reasonably clear, questions only when truly ambiguous
- [ ] **No tentative or "possible" BrainLifts** - committed to either proposing or questioning
- [ ] For each proposed BrainLift, the purpose statement is clear and identifies the expertise gap (not just restating the goal)
- [ ] For each proposed BrainLift, in/out scope is defined (minimum 1 item each, more if context provides)
- [ ] For execution-only tasks, the reasoning is explained
- [ ] When problems/expertise gaps are genuinely ambiguous, specific clarifying questions are asked (not generic ones)
- [ ] Reasonable inferences made from document context without inventing problems
- [ ] Problems vs. outcomes are clearly distinguished

---

**Quarterly Plan Document**:
If the user didn't provide the quarterly plan document, do not continue and ask them to do so.

---

Please produce the decomposition analysis following the methodology and output format above. Save your result to `results/{context_file_name+_results}.md`
