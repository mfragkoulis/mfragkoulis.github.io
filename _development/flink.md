---
title: "High availability in Apache Flink"
permalink: /development/flink.md
excerpt: "Apache Flink is a stream processing system offering high-throughput and low-latency processing of millions events per second with exactly-once processing guarantees even in face of failures. However, Flink's failover strategy stops data processing, resets the whole job graph, and resumes from the latest checkpoint assuming a replayable input source such as Apache Kafka. This is not suitable for mission-critical jobs that need fast recovery or large-scale jobs running on tens or hundreds of machines where the probability of any node failing becomes so big that may result in subsequent failures that leave the job with no progress between failures.

This project provides a faster recovery strategy for higher availability. The strategy sets up standby tasks that mirror running tasks and receive the state snapshots of the running tasks upon each checkpoint. Tasks that produce output log it until the next checkpoint. When a failure happens the standby task that mirrors the failed running task comes into play and substitutes the failed task. It requests the in-flight log from its upstream tasks and starts processing thereby reducing the failure only to the tasks that failed. This recovery strategy guarantess at-least-once processing since there may be records that will be processed twice, once by the failed task and once by the standby task that substtituted it. Techniques like causal logging can help strengthening the processing guarantee to exactly-once. Check out the work by Pedro Silvestre ([https://github.com/PSilvestre](https://github.com/PSilvestre)).

1. Github repo: [https://github.com/tud-delta/flink](https://github.com/tud-delta/flink)
"
collection: development
---
