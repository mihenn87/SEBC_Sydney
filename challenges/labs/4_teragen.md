## Teragen
---

```bash
[cate@ip-172-31-10-82 root]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar teragen -D dfs.blocksize=16M -D mapreduce.map.memory.mb=512 65536000 /user/cate/tgen
17/05/05 05:05:47 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-10-82.eu-central-1.compute.internal/172.31.10.82:8032
17/05/05 05:05:47 INFO terasort.TeraGen: Generating 65536000 using 2
17/05/05 05:05:47 INFO mapreduce.JobSubmitter: number of splits:2
17/05/05 05:05:48 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493973855667_0001
17/05/05 05:05:48 INFO impl.YarnClientImpl: Submitted application application_1493973855667_0001
17/05/05 05:05:48 INFO mapreduce.Job: The url to track the job: http://ip-172-31-10-82.eu-central-1.compute.internal:8088/proxy/application_1493973855667_0001/
17/05/05 05:05:48 INFO mapreduce.Job: Running job: job_1493973855667_0001
17/05/05 05:05:55 INFO mapreduce.Job: Job job_1493973855667_0001 running in uber mode : false
17/05/05 05:05:55 INFO mapreduce.Job:  map 0% reduce 0%
17/05/05 05:06:14 INFO mapreduce.Job:  map 21% reduce 0%
17/05/05 05:06:20 INFO mapreduce.Job:  map 26% reduce 0%
17/05/05 05:06:27 INFO mapreduce.Job:  map 32% reduce 0%
17/05/05 05:06:33 INFO mapreduce.Job:  map 38% reduce 0%
17/05/05 05:06:39 INFO mapreduce.Job:  map 43% reduce 0%
17/05/05 05:06:45 INFO mapreduce.Job:  map 49% reduce 0%
17/05/05 05:06:51 INFO mapreduce.Job:  map 55% reduce 0%
17/05/05 05:06:57 INFO mapreduce.Job:  map 60% reduce 0%
17/05/05 05:07:03 INFO mapreduce.Job:  map 66% reduce 0%
17/05/05 05:07:09 INFO mapreduce.Job:  map 70% reduce 0%
17/05/05 05:07:15 INFO mapreduce.Job:  map 76% reduce 0%
17/05/05 05:07:21 INFO mapreduce.Job:  map 83% reduce 0%
17/05/05 05:07:27 INFO mapreduce.Job:  map 88% reduce 0%
17/05/05 05:07:33 INFO mapreduce.Job:  map 94% reduce 0%
17/05/05 05:07:39 INFO mapreduce.Job:  map 100% reduce 0%
17/05/05 05:07:39 INFO mapreduce.Job: Job job_1493973855667_0001 completed successfully
17/05/05 05:07:39 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=249926
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=170
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=8
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=202987
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=202987
                Total vcore-seconds taken by all map tasks=202987
                Total megabyte-seconds taken by all map tasks=207858688
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1208
                CPU time spent (ms)=93490
                Physical memory (bytes) snapshot=330399744
                Virtual memory (bytes) snapshot=2278608896
                Total committed heap usage (bytes)=393216000
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

```
				
## Time
---

```bash
real    1m54.934s
user    0m6.113s
sys     0m0.291s
```

## ls
---

```bash
[cate@ip-172-31-10-82 root]$ hdfs dfs -ls /user/cate/tgen
Found 3 items
-rw-r--r--   3 cate cate          0 2017-05-05 05:07 /user/cate/tgen/_SUCCESS
-rw-r--r--   3 cate cate 3276800000 2017-05-05 05:07 /user/cate/tgen/part-m-00000
-rw-r--r--   3 cate cate 3276800000 2017-05-05 05:07 /user/cate/tgen/part-m-00001
[cate@ip-172-31-10-82 root]$

```