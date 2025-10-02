# SparkStreaming
Spark Streaming learning

## What is streaming?
- It's an ever growing table
- Before Data were processed after having all the rows filled, but now we don't have time to wait! Data keeps flowing in and we need to process it.

## Apache Spark
- Spark takes **micro batches** periodically (1 sec, 1 millisec ...) and update the result.
### Stateless Transformation
- It will append the input
- Doesn't require context of the resulting table

### Stateful Transformation
- It modifies the result
- For example, group bu functions will be a stateful transformation. Since it needs to know the context of the resulting table to grow the groups with new input values.
