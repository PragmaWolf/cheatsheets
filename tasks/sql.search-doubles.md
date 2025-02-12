# SQL. Выбрать дублирующиеся данные

---

## Решение 1

```sql
SELECT *, COUNT(*) OVER (PARTITION BY column_name) as cnt
FROM table_name
HAVING cnt > 1;
```

---

## Решение 2

```sql
SELECT column_name, COUNT(*) AS cnt
FROM table_name
GROUP BY column_name
HAVING cnt > 1;
```
