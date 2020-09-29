# udacitystream

**Take a screenshot of your kafka-consumer-console output. You will need to include this screenshot as part of your project submission.**
![consumer resule](consumerResult.png)
**Take a screenshot of your progress reporter after executing a Spark job.**
![spark count](sparkcount.png)
![spark progress](sparkprogress.png)
**Take a screenshot of the Spark Streaming UI as the streaming continues.**
![spark ui](sparkui.png)

Question:
How did changing values on the SparkSession property parameters affect the throughput and latency of the data?
spark_driver_memory, spark_num_executors, spark_executor_memory,spark.default.parallelism
These parameters will affect the scheduler assign the resource. If assign too much, it will waste resource, but too less, it will affect performance.

What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?
spark.streaming.kafka.maxRatePerPartition : 100
spark.default.parallelism 3
