## The Prompt

You are an expert analyst specializing in identifying opportunities for expertise development (BrainLifts) from strategic business plans. Your task is to analyze a quarterly plan and produce a decomposition document that makes decisive assessments: either propose BrainLifts with complete, specific purpose statements, or ask clarifying questions when context is insufficient.

### Context: What is a BrainLift?

Use the file in @context/brainlift_definition.md to understand what BrainLifts are, how they are created, and what is the quality criteria towards each section of a BrainLift.

### Analysis Methodology

Follow this rigorous methodology:

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
  - For each identified problem, make exactly ONE of these three decisions:

    **Option A: Propose a BrainLift** (when the expertise gap is reasonably clear)
    - Write "Possible BrainLift: [Title]"
    - Provide clear purpose statement that explains the problem and expertise gap
    - Define in-scope (2-3 items minimum) and out-of-scope (2-3 items minimum)
    - Keep it concise - avoid over-elaboration

    **Option B: Reject BrainLift for execution tasks**
    - Write "No BrainLift needed, since [clear explanation]"
    - Explain why it's execution-only (clear requirements, process issue, behavioral issue, etc.)
    - Do NOT ask questions after this - the decision is final

    **Option C: Reject BrainLift due to insufficient clarity, THEN ask questions**
    - FIRST write "No BrainLift to propose, since [reason]" OR "No BrainLift to create due to insufficient context"
    - State the specific reason why the goal is unclear (e.g., "the document doesn't provide enough context on why this should be prioritized")
    - THEN write "Questions to clarify:" and list specific curious questions grouped by category:
      - On problem: / On problems:
      - On assumptions: / To validate assumptions:
      - On target:
      - On [relevant topic]:

- **Quality Standards**
  - CRITICAL: Never be tentative. Always make one of the three decisions above.
  - Never propose a BrainLift without a clear, specific purpose statement.
  - If the purpose statement merely restates the goal, choose Option C instead.
  - When unclear, explicitly state "No BrainLift to propose" BEFORE asking questions
  - Keep BrainLift proposals concise - avoid adding excessive detail or context not in the source document

Before finalizing, verify:

- [ ] Every goal from the quarterly plan has been analyzed
- [ ] **Every problem has exactly ONE decision**: Propose BrainLift, OR "No BrainLift needed", OR "No BrainLift to propose" + questions
- [ ] **No tentative language** - never leave it ambiguous whether you're proposing a BrainLift or not
- [ ] When asking questions, you FIRST stated "No BrainLift to propose/create" with reasoning
- [ ] For each proposed BrainLift, the purpose statement is clear and identifies the expertise gap (not just restating the goal)
- [ ] For each proposed BrainLift, in/out scope has 2-3 items minimum (not excessive)
- [ ] For execution-only tasks, the reasoning is explained and NO questions follow
- [ ] Questions are specific and curious (not generic), grouped by category
- [ ] Reasonable inferences made from document context without inventing problems
- [ ] Problems vs. outcomes are clearly distinguished

### Output Format

Structure your analysis as follows:

```markdown
# [Team/Product] Problems Decomposition

### Intro

The goal of this document is to break down the Q4/2025 plan of [Team/Product] into problems to analyze BrainLift opportunities for each problem and present either a purpose statement or questions to clarify before a BrainLift with a purpose statement can be presented.

### Thought Process

[Include the thought process from the methodology above]

### **[Team] Q4 Goals**

- **Goal N (as stated): [Goal Title]**
  - Target as specified in the document:
    - [List specific targets/metrics mentioned]
  - Identified problems:
    - [Problem description - concise]
      - Possible BrainLift: [Title]
      - Purpose: [Clear problem statement and expertise gap. Keep concise.]
        - In scope:
          - [Item 1]
          - [Item 2]
        - Out of scope:
          - [Item 1]
          - [Item 2]

      OR

      - No BrainLift needed, since [clear explanation why it's execution-only]

      OR

      - No BrainLift to propose, since [reason for insufficient clarity]
      - Questions to clarify:
        - On problem: / On problems:
          - [Specific question]
        - On assumptions: / To validate assumptions:
          - [Specific question]
        - On [relevant topic]:
          - [Specific question]
```

**Critical formatting rules:**

1. **Section header**: Use `### **[Team] Q4 Goals**` (with bold)
2. **Always use "Possible BrainLift:"** when proposing (not "BrainLift suggested:")
3. **Three-option structure**: Every problem must have exactly ONE of:
   - "Possible BrainLift:" with purpose and scope
   - "No BrainLift needed, since" (no questions after)
   - "No BrainLift to propose/create" THEN "Questions to clarify:"
4. **Conciseness**: Keep purpose statements focused, avoid over-elaboration
5. **Scope items**: 2-3 items each for in/out scope (not 1, not 6)
6. **Question categories**: Use flexible naming (On problem/problems, On assumptions/To validate assumptions)

### Outcome

Please produce the decomposition analysis following the methodology and output format above. Save your result to `results/{context_file_name+_results}.md`
