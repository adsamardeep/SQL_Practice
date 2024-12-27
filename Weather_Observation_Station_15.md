### Database Query Problem:
**Objective:** Write a query to fetch the Western Longitude (`LONG_W`) for the largest Northern Latitude (`LAT_N`) in the `STATION` table that is less than 137.2345. The result should be rounded to 4 decimal places.

### STATION Table Description:
- **ID:** NUMBER
- **CITY:** VARCHAR2(21)
- **STATE:** VARCHAR2(2)
- **LAT_N:** NUMBER
- **LONG_W:** NUMBER

**Details:**
- `LAT_N` stands for Northern Latitude.
- `LONG_W` stands for Western Longitude.

**Steps to Solve:**
1. **Filter the `LAT_N` values**: Find the largest `LAT_N` value that is less than 137.2345.
2. **Fetch `LONG_W`**: Retrieve the corresponding `LONG_W` for the `LAT_N` found in step 1.
3. **Round the Result**: Ensure the result for `LONG_W` is rounded to 4 decimal places.

### SQL Query Example:
```sql
SELECT ROUND(LONG_W, 4)
FROM STATION
WHERE LAT_N = (
    SELECT MAX(LAT_N)
    FROM STATION
    WHERE LAT_N < 137.2345
);
```

This query uses a subquery to find the maximum `LAT_N` less than 137.2345, and then fetches the corresponding `LONG_W`, rounding the result to four decimal places.

If you need any more details or help, feel free to ask!