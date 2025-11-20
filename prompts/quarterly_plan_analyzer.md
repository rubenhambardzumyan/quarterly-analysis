# Quarterly Plan Analyzer

## Your Task

Analyze a quarterly plan to identify BrainLift opportunities (areas where expertise needs to be developed or documented).

## What's a BrainLift?

A BrainLift is a documented area of expertise that helps someone make better decisions. It captures:
- The problem that needs expert judgment (not just execution)
- The specific expertise gap
- What's in scope and out of scope

For more context, see @context/brainlift_definition.md, but don't let it overcomplicate your analysis.

## How to Analyze

For each goal in the quarterly plan:

**If you see a clear expertise gap:**
- **Possible BrainLift:** [Title]
- **Purpose:** 2-3 sentences explaining what problem exists and what expertise would solve it
- **In scope:** 2-3 items
- **Out of scope:** 2-3 items

**If it's clearly just execution (no expertise needed):**
- **No BrainLift needed** - [one sentence why]

**If you're unclear what the problem is:**
- **Questions:** Ask 1-2 specific questions to understand better

## Guidelines

- **Be decisive.** Don't hedge with "potentially" or "might require."
- **Be concise.** Purpose statements should be 2-3 sentences, not paragraphs.
- **Be human.** Write like you're analyzing this for a colleague, not filling out a form.
- **Make reasonable inferences.** Don't ask questions just because every detail isn't spelled out.
- **Don't dump questions.** If unclear, ask 1-2 focused questions, not 10.

## Output Format

```markdown
# [Team/Product] Problems Decomposition

### **[Team] Q4 Goals**

- **Goal 1: [Goal Title]**
  - Target: [key metrics from document]
  - [Your analysis - BrainLift proposal, dismissal, or questions]

- **Goal 2: [Goal Title]**
  - Target: [key metrics from document]
  - [Your analysis]
```

Keep it readable and useful. The goal is to help someone understand what expertise they need to develop, not to follow a bureaucratic checklist.

## Example

See @context/crossover_decomposition.md for what good analysis looks like.

Save your result to `results/{plan_name}_results.md`
