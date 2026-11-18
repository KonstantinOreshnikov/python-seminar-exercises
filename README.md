# Python Seminar Exercises

A compact collection of Python exercises completed during seminar-based learning.

## Focus

- Python fundamentals
- Problem solving
- Functions and data structures
- Practice-oriented assignments

## Status

Completed learning repository retained for reference.

## From small exercises to reusable analytical functions

These files preserve early Python seminar practice. They are **historical learning exercises**; their presence is not evidence of production readiness or a recent test run.

### Skills developed

| Concept | Basic exercise | Transfer to reporting / automation |
|---|---|---|
| Loops | Count matching values | Validate rows in a synthetic CSV |
| Conditions | Check thresholds | Flag invalid or missing inputs |
| Lists and dictionaries | Group observations | Prepare a small summary |
| Functions | Separate calculation from input | Reuse and test transformations |
| Errors | Reject unexpected inputs | Fail a scheduled job clearly |
| Tests | Assert boundary behavior | Prevent regression after a change |

### Example: a fictional summary

```python
from collections import Counter

events = ["opened", "closed", "opened", "review"]
counts = Counter(events)
assert counts["opened"] == 2
assert sum(counts.values()) == len(events)
```

Next step: read a tiny invented CSV, validate keys, group by period and reconcile the grouped total with the source. The [Python Learning Lab](https://github.com/KonstantinOreshnikov/python-lessons-geekbrains) contains a more structured route and a synthetic reporting pipeline.

### Quality and boundaries

Practice input handling, deterministic tests and clear error messages. Do not turn a homework exercise into a database job without checking field types, population, duplicate handling and permissions. Existing seminar scripts remain untouched.

**RU:** семинарские задачи показывают, как базовые циклы, коллекции и функции развиваются в Python-валидацию данных, отчёты и автоматизацию.

References: [Python tutorial](https://docs.python.org/3/tutorial/), [collections](https://docs.python.org/3/library/collections.html).
