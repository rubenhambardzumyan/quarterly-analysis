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

Analysis results are saved to `results/{plan_name}_decomposition.md`
