
# SQL Interview Question Bank (64 Questions)

## Foundations (DDL, ALTER, Constraints, DML)

1. What is DDL and how is it different from DML in terms of behavior?
2. Why are DDL statements often auto-commit?
3. Can DDL be rolled back? Why or why not?
4. Why is ALTER considered more dangerous than UPDATE in production?
5. What happens internally when you add a column to a large table?
6. Is renaming a table a DDL or DML operation? Why?
7. Is TRUNCATE DDL or DML? Defend your answer.
8. Does CREATE TABLE AS SELECT count as DDL or DML?
9. What are the different types of ALTER operations?
10. Which ALTER operations are metadata-only vs data-rewriting?
11. What happens if you add a NOT NULL column to an existing table?
12. Why can changing a column’s data type cause a full table rewrite?
13. What risks exist when dropping a column?
14. Why is ALTER risky on tables with indexes and foreign keys?
15. How would you safely add a NOT NULL column to a table with 1B rows?
16. How would you change a column from VARCHAR to INT safely?

## Querying Core (SELECT, JOIN, GROUP BY)

17. What is the execution order of a SELECT query?
18. What is the difference between WHERE and HAVING?
19. What are the different types of JOINs and when would you use each?
20. What happens when you JOIN on NULL values?
21. How does GROUP BY work internally?
22. Why must every non-aggregated column appear in GROUP BY?
23. What is the difference between COUNT(*) and COUNT(column)?
24. How does ORDER BY interact with indexes?
25. What are common GROUP BY mistakes in interviews?
26. How do LEFT JOINs become INNER JOINs accidentally?
27. When would you use UNION vs UNION ALL?
28. How does LIMIT/OFFSET affect performance?

## Intermediate (Subqueries, CTEs, Window Functions)

29. What is the difference between a subquery and a CTE?
30. When is a correlated subquery evaluated?
31. Why are correlated subqueries often slow?
32. Can a CTE be referenced multiple times in a query?
33. Are CTEs always materialized?
34. What is a window function?
35. How are window functions different from GROUP BY?
36. What does PARTITION BY do?
37. What does ORDER BY do inside a window function?
38. Difference between ROW_NUMBER, RANK, and DENSE_RANK?
39. How do you find the second highest value using a window function?
40. What are common window function interview traps?
41. Can window functions be used in WHERE? Why or why not?
42. How would you rewrite a subquery using a window function?

## Advanced / Staff (Performance, Migrations, Tradeoffs)

43. How does the query planner choose an execution plan?
44. What is an index and how does it help performance?
45. When can indexes hurt performance?
46. What is an index-only scan?
47. How do you identify slow queries?
48. What is a table lock vs row lock?
49. How do long-running transactions affect the system?
50. What is transaction isolation and why does it matter?
51. How would you delete millions of rows safely?
52. How would you backfill data in production?
53. What is a zero-downtime migration?
54. How do you avoid blocking writes during schema changes?
55. How do foreign keys impact write scalability?
56. Why do some large systems avoid foreign keys?
57. How do you enforce data integrity without constraints?
58. What tradeoffs exist between database constraints and application logic?
59. How would you recover from an accidental DELETE?
60. How would you design auditability for data changes?
61. How do schema decisions impact long-term velocity?
62. When should correctness live in the DB vs the application?
63. How do you reason about performance vs correctness tradeoffs?
64. What signals distinguish a senior vs staff-level SQL answer?
