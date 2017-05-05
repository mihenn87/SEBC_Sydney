## Terasort

```bash
[cate@ip-172-31-15-57 root]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar terasort /user/cate/tgen /user/cate/tsort640m
17/05/05 05:43:46 INFO terasort.TeraSort: starting
17/05/05 05:43:48 INFO hdfs.DFSClient: Created token for cate: HDFS_DELEGATION_TOKEN owner=cate@MIHENN87.AU, renewer=yarn, realUser=, issueDate=1493977427996, maxDate=1494582227996, sequenceNumber=1, masterKeyId=2 on 172.31.10.82:8020
17/05/05 05:43:48 INFO security.TokenCache: Got dt for hdfs://ip-172-31-10-82.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.10.82:8020, Ident: (token for cate: HDFS_DELEGATION_TOKEN owner=cate@MIHENN87.AU, renewer=yarn, realUser=, issueDate=1493977427996, maxDate=1494582227996, sequenceNumber=1, masterKeyId=2)
17/05/05 05:43:48 INFO input.FileInputFormat: Total input paths to process : 2
Spent 435ms computing base-splits.
Spent 7ms computing TeraScheduler splits.
Computing input splits took 442ms
Sampling 10 splits of 392
Making 8 from 100000 sampled records
Computing parititions took 1021ms
Spent 1466ms computing partitions.
17/05/05 05:43:49 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-10-82.eu-central-1.compute.internal/172.31.10.82:8032
17/05/05 05:43:49 INFO mapreduce.JobSubmitter: number of splits:392
17/05/05 05:43:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493976890859_0001
17/05/05 05:43:49 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.10.82:8020, Ident: (token for cate: HDFS_DELEGATION_TOKEN owner=cate@MIHENN87.AU, renewer=yarn, realUser=, issueDate=1493977427996, maxDate=1494582227996, sequenceNumber=1, masterKeyId=2)
17/05/05 05:43:51 INFO impl.YarnClientImpl: Submitted application application_1493976890859_0001
17/05/05 05:43:51 INFO mapreduce.Job: The url to track the job: http://ip-172-31-10-82.eu-central-1.compute.internal:8088/proxy/application_1493976890859_0001/
17/05/05 05:43:51 INFO mapreduce.Job: Running job: job_1493976890859_0001
17/05/05 05:44:00 INFO mapreduce.Job: Job job_1493976890859_0001 running in uber mode : false
17/05/05 05:44:00 INFO mapreduce.Job:  map 0% reduce 0%
17/05/05 05:44:11 INFO mapreduce.Job:  map 1% reduce 0%
17/05/05 05:44:13 INFO mapreduce.Job:  map 2% reduce 0%
17/05/05 05:44:19 INFO mapreduce.Job:  map 3% reduce 0%
17/05/05 05:44:20 INFO mapreduce.Job:  map 4% reduce 0%
17/05/05 05:44:27 INFO mapreduce.Job:  map 6% reduce 0%
17/05/05 05:44:34 INFO mapreduce.Job:  map 8% reduce 0%
17/05/05 05:44:41 INFO mapreduce.Job:  map 9% reduce 0%
17/05/05 05:44:43 INFO mapreduce.Job:  map 10% reduce 0%
17/05/05 05:44:48 INFO mapreduce.Job:  map 11% reduce 0%
17/05/05 05:44:53 INFO mapreduce.Job:  map 12% reduce 0%
17/05/05 05:44:55 INFO mapreduce.Job:  map 13% reduce 0%
17/05/05 05:44:58 INFO mapreduce.Job:  map 14% reduce 0%
17/05/05 05:45:02 INFO mapreduce.Job:  map 15% reduce 0%
17/05/05 05:45:08 INFO mapreduce.Job:  map 16% reduce 0%
17/05/05 05:45:09 INFO mapreduce.Job:  map 17% reduce 0%
17/05/05 05:45:15 INFO mapreduce.Job:  map 18% reduce 0%
17/05/05 05:45:16 INFO mapreduce.Job:  map 19% reduce 0%
17/05/05 05:45:23 INFO mapreduce.Job:  map 20% reduce 0%
17/05/05 05:45:24 INFO mapreduce.Job:  map 21% reduce 0%
17/05/05 05:45:30 INFO mapreduce.Job:  map 22% reduce 0%
17/05/05 05:45:31 INFO mapreduce.Job:  map 23% reduce 0%
17/05/05 05:45:37 INFO mapreduce.Job:  map 24% reduce 0%
17/05/05 05:45:39 INFO mapreduce.Job:  map 25% reduce 0%
17/05/05 05:45:44 INFO mapreduce.Job:  map 26% reduce 0%
17/05/05 05:45:45 INFO mapreduce.Job:  map 27% reduce 0%
17/05/05 05:45:51 INFO mapreduce.Job:  map 28% reduce 0%
17/05/05 05:45:53 INFO mapreduce.Job:  map 29% reduce 0%
17/05/05 05:45:58 INFO mapreduce.Job:  map 30% reduce 0%
17/05/05 05:45:59 INFO mapreduce.Job:  map 31% reduce 0%
17/05/05 05:46:05 INFO mapreduce.Job:  map 32% reduce 0%
17/05/05 05:46:11 INFO mapreduce.Job:  map 33% reduce 0%
17/05/05 05:46:13 INFO mapreduce.Job:  map 34% reduce 0%
17/05/05 05:46:19 INFO mapreduce.Job:  map 35% reduce 0%
17/05/05 05:46:20 INFO mapreduce.Job:  map 36% reduce 0%
17/05/05 05:46:26 INFO mapreduce.Job:  map 37% reduce 0%
17/05/05 05:46:27 INFO mapreduce.Job:  map 38% reduce 0%
17/05/05 05:46:33 INFO mapreduce.Job:  map 39% reduce 0%
17/05/05 05:46:42 INFO mapreduce.Job:  map 40% reduce 0%
17/05/05 05:46:46 INFO mapreduce.Job:  map 41% reduce 0%
17/05/05 05:46:50 INFO mapreduce.Job:  map 42% reduce 0%
17/05/05 05:46:55 INFO mapreduce.Job:  map 43% reduce 0%
17/05/05 05:46:58 INFO mapreduce.Job:  map 44% reduce 0%
17/05/05 05:47:01 INFO mapreduce.Job:  map 45% reduce 0%
17/05/05 05:47:06 INFO mapreduce.Job:  map 46% reduce 0%
17/05/05 05:47:08 INFO mapreduce.Job:  map 47% reduce 0%
17/05/05 05:47:14 INFO mapreduce.Job:  map 48% reduce 0%
17/05/05 05:47:17 INFO mapreduce.Job:  map 49% reduce 0%
17/05/05 05:47:21 INFO mapreduce.Job:  map 50% reduce 0%
17/05/05 05:47:22 INFO mapreduce.Job:  map 51% reduce 0%
17/05/05 05:47:27 INFO mapreduce.Job:  map 52% reduce 0%
17/05/05 05:47:30 INFO mapreduce.Job:  map 53% reduce 0%
17/05/05 05:47:35 INFO mapreduce.Job:  map 54% reduce 0%
17/05/05 05:47:37 INFO mapreduce.Job:  map 55% reduce 0%
17/05/05 05:47:42 INFO mapreduce.Job:  map 56% reduce 0%
17/05/05 05:47:44 INFO mapreduce.Job:  map 57% reduce 0%
17/05/05 05:47:49 INFO mapreduce.Job:  map 58% reduce 0%
17/05/05 05:47:51 INFO mapreduce.Job:  map 59% reduce 0%
17/05/05 05:47:56 INFO mapreduce.Job:  map 60% reduce 0%
17/05/05 05:47:57 INFO mapreduce.Job:  map 61% reduce 0%
17/05/05 05:48:03 INFO mapreduce.Job:  map 62% reduce 0%
17/05/05 05:48:04 INFO mapreduce.Job:  map 63% reduce 0%
17/05/05 05:48:11 INFO mapreduce.Job:  map 64% reduce 0%
17/05/05 05:48:13 INFO mapreduce.Job:  map 65% reduce 0%
17/05/05 05:48:18 INFO mapreduce.Job:  map 66% reduce 0%
17/05/05 05:48:22 INFO mapreduce.Job:  map 67% reduce 0%
17/05/05 05:48:25 INFO mapreduce.Job:  map 68% reduce 0%
17/05/05 05:48:32 INFO mapreduce.Job:  map 70% reduce 0%
17/05/05 05:48:39 INFO mapreduce.Job:  map 72% reduce 0%
17/05/05 05:48:46 INFO mapreduce.Job:  map 74% reduce 0%
17/05/05 05:48:52 INFO mapreduce.Job:  map 76% reduce 0%
17/05/05 05:49:00 INFO mapreduce.Job:  map 77% reduce 0%
17/05/05 05:49:01 INFO mapreduce.Job:  map 78% reduce 0%
17/05/05 05:49:07 INFO mapreduce.Job:  map 79% reduce 0%
17/05/05 05:49:09 INFO mapreduce.Job:  map 80% reduce 0%
17/05/05 05:49:14 INFO mapreduce.Job:  map 81% reduce 0%
17/05/05 05:49:18 INFO mapreduce.Job:  map 82% reduce 0%
17/05/05 05:49:21 INFO mapreduce.Job:  map 83% reduce 0%
17/05/05 05:49:28 INFO mapreduce.Job:  map 84% reduce 0%
17/05/05 05:49:34 INFO mapreduce.Job:  map 85% reduce 0%
17/05/05 05:49:38 INFO mapreduce.Job:  map 85% reduce 14%
17/05/05 05:49:40 INFO mapreduce.Job:  map 86% reduce 14%
17/05/05 05:49:48 INFO mapreduce.Job:  map 87% reduce 14%
17/05/05 05:49:53 INFO mapreduce.Job:  map 88% reduce 14%
17/05/05 05:49:56 INFO mapreduce.Job:  map 88% reduce 15%
17/05/05 05:49:59 INFO mapreduce.Job:  map 89% reduce 15%
17/05/05 05:50:05 INFO mapreduce.Job:  map 90% reduce 15%
17/05/05 05:50:13 INFO mapreduce.Job:  map 91% reduce 15%
17/05/05 05:50:19 INFO mapreduce.Job:  map 92% reduce 15%
17/05/05 05:50:25 INFO mapreduce.Job:  map 93% reduce 15%
17/05/05 05:50:32 INFO mapreduce.Job:  map 93% reduce 16%
17/05/05 05:50:33 INFO mapreduce.Job:  map 94% reduce 16%
17/05/05 05:50:39 INFO mapreduce.Job:  map 95% reduce 16%
17/05/05 05:50:45 INFO mapreduce.Job:  map 96% reduce 16%
17/05/05 05:50:53 INFO mapreduce.Job:  map 97% reduce 16%
17/05/05 05:50:59 INFO mapreduce.Job:  map 98% reduce 16%
17/05/05 05:51:05 INFO mapreduce.Job:  map 99% reduce 16%
17/05/05 05:51:14 INFO mapreduce.Job:  map 100% reduce 16%
17/05/05 05:51:15 INFO mapreduce.Job:  map 100% reduce 17%
17/05/05 05:51:21 INFO mapreduce.Job:  map 100% reduce 37%
17/05/05 05:51:27 INFO mapreduce.Job:  map 100% reduce 53%
17/05/05 05:51:29 INFO mapreduce.Job:  map 100% reduce 55%
17/05/05 05:51:30 INFO mapreduce.Job:  map 100% reduce 65%
17/05/05 05:51:32 INFO mapreduce.Job:  map 100% reduce 73%
17/05/05 05:51:33 INFO mapreduce.Job:  map 100% reduce 77%
17/05/05 05:51:36 INFO mapreduce.Job:  map 100% reduce 80%
17/05/05 05:51:37 INFO mapreduce.Job:  map 100% reduce 81%
17/05/05 05:51:38 INFO mapreduce.Job:  map 100% reduce 84%
17/05/05 05:51:39 INFO mapreduce.Job:  map 100% reduce 88%
17/05/05 05:51:46 INFO mapreduce.Job:  map 100% reduce 96%
17/05/05 05:51:52 INFO mapreduce.Job:  map 100% reduce 99%
17/05/05 05:51:53 INFO mapreduce.Job:  map 100% reduce 100%
17/05/05 05:51:54 INFO mapreduce.Job: Job job_1493976890859_0001 completed successfully
17/05/05 05:51:54 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2908572482
                FILE: Number of bytes written=5802547738
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553658800
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=1200
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=392
                Launched reduce tasks=8
                Data-local map tasks=390
                Rack-local map tasks=2
                Total time spent by all maps in occupied slots (ms)=2100835
                Total time spent by all reduces in occupied slots (ms)=602306
                Total time spent by all map tasks (ms)=2100835
                Total time spent by all reduce tasks (ms)=602306
                Total vcore-seconds taken by all map tasks=2100835
                Total vcore-seconds taken by all reduce tasks=602306
                Total megabyte-seconds taken by all map tasks=2151255040
                Total megabyte-seconds taken by all reduce tasks=616761344
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2843088150
                Input split bytes=58800
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2843088150
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =3136
                Failed Shuffles=0
                Merged Map outputs=3136
                GC time elapsed (ms)=28468
                CPU time spent (ms)=1330980
                Physical memory (bytes) snapshot=190176018432
                Virtual memory (bytes) snapshot=635163385856
                Total committed heap usage (bytes)=224334970880
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/05/05 05:51:54 INFO terasort.TeraSort: done
[cate@ip-172-31-15-57 root]$
```