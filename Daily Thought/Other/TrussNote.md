# Truss Note
### Fuzzy Search
```sql
WITH similarity_data AS (
  SELECT *, word_similarity(name, 'misspeled_word') AS similarity_score
  FROM projects
)

SELECT *
FROM similarity_data
WHERE similarity_score > (0.3 + (length('misspeled_word')::float / 100)) -- Adjust the threshold as needed
ORDER BY similarity_score DESC;
```
