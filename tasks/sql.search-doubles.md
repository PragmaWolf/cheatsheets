# SQL. Выбрать дублирующиеся данные

Необходимо выбрать из таблицы дублирующиеся записи.

[К оглавлению](../README.md)

---

## Решение 1

```sql
SELECT column_name, COUNT(*) OVER (PARTITION BY column_name) as cnt
FROM table_name
HAVING cnt > 1;
```

[К оглавлению](../README.md)

---

## Решение 2

```sql
SELECT column_name, COUNT(*) AS cnt
FROM table_name
GROUP BY column_name
HAVING cnt > 1;
```

[К оглавлению](../README.md)
