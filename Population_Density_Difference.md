
**Question:**
Query the difference between the maximum and minimum populations in the CITY table.

**Solution:**

1. **Schema:**

The CITY table is described as follows:

| Field       | Type          |
|-------------|---------------|
| ID          | NUMBER        |
| NAME        | VARCHAR2(17)  |
| COUNTRYCODE | VARCHAR2(3)   |
| DISTRICT    | VARCHAR2(20)  |
| POPULATION  | NUMBER        |

2. **SQL Query:**

To find the difference between the maximum and minimum populations in the CITY table, you can use the following SQL query:

```sql
SELECT MAX(POPULATION) - MIN(POPULATION) AS PopulationDifference
FROM CITY;
```

3. **Explanation:**

- `MAX(POPULATION)` retrieves the maximum population value from the CITY table.
- `MIN(POPULATION)` retrieves the minimum population value from the CITY table.
- Subtracting `MIN(POPULATION)` from `MAX(POPULATION)` computes the difference between these two values.
- `AS PopulationDifference` renames the resulting difference for clarity in the output.

**Example Output:**

| PopulationDifference |
|----------------------|
| 1234567              |

In this example, `1234567` represents the calculated difference between the highest and lowest population values in the CITY table.

---

Feel free to reach out if you need further assistance or additional queries!