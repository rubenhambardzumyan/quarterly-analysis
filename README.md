# Quarterly Plan BrainLift Analyzer

This repository contains a prompt-based analysis system for identifying BrainLift opportunities from quarterly business plans.

## What it does

The analyzer examines quarterly plans to:

- **Extract goals** and distinguish between problems vs. outcomes
- **Identify expertise gaps** that require BrainLift development
- **Propose BrainLifts** with clear purpose statements, in-scope, and out-of-scope items
- **Flag execution-only tasks** that don't require expertise development
- **Ask clarifying questions** when context is insufficient

## How to use

Run the analyzer prompt on any quarterly plan document:

```
Run @prompts/quarterly_plan_analyzer.md on {quarterly_plan_file_source}.md
```

**Example:**

```
Run @prompts/quarterly_plan_analyzer.md on @q4_plans/dragos_crossover.md
```

## Context Files

- **`context/brainlift_definition.md`** - Defines what BrainLifts are and quality criteria
- **`context/crossover_decomposition.md`** - Example analysis showing the methodology in action

## Output

Analysis results are saved to `results/{plan_name}_decomposition.md` with:

- Goal-by-goal breakdown
- Problem identification
- BrainLift proposals or clarifying questions
- Clear distinction between expertise development vs. execution tasks
