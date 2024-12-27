---

# SQL Practice Questions

## Overview

Welcome to the **SQL Practice Questions** repository! This is a collection of SQL problems designed to help you improve your SQL skills, ranging from basic queries to more complex challenges. Whether you're preparing for interviews or just practicing, this repo has a variety of questions to work on.

## Structure

- **Basic:** Simple queries, SELECT statements, filtering.
- **Intermediate:** Joins, subqueries, aggregations.
- **Advanced:** Window functions, CTEs, optimization.

## Contributing

1. Fork and clone the repo.
2. Add a question in the appropriate folder (e.g., `/basic`, `/intermediate`, `/advanced`).
3. Include the SQL query and an explanation.
4. Push changes and submit a pull request.

## Example Question

**Find the difference between the maximum and minimum population:**

```sql
SELECT MAX(population) - MIN(population) AS population_difference
FROM city;
```

**Explanation:** This query calculates the difference between the highest and lowest population using `MAX()` and `MIN()`.

## License

This repository is open-source. Feel free to contribute!

---
