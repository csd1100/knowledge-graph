- number of unique values in specific column
- If there are multiple unique values i.e. High Cardinality it is better to have index for those values
- Low Cardinality low amount of unique values
- High Cardinality means efficient searching

- Cardinality matters for number of comparisons even after index because if indexed values are multiple rows we have to do that many comparisons
- For High Cardinality after index O(log n) for B-Trees the comparison can be just few rows

```
Index path cost = O(log n) descent + m × random_io_cost
Full scan cost  = n × seq_io_cost   
```