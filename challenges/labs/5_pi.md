## Pi
```bash
[jemaine@ip-172-31-9-185 root]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-mapreduce/hadoop-mapreduce-examples.jar pi 4 200
Number of Maps  = 4
Samples per Map = 200
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Starting Job
17/05/05 05:46:09 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-10-82.eu-central-1.compute.internal/172.31.10.82:8032
17/05/05 05:46:09 INFO hdfs.DFSClient: Created token for jemaine: HDFS_DELEGATION_TOKEN owner=jemaine@MIHENN87.AU, renewer=yarn, realUser=, issueDate=1493977569868, maxDate=1494582369868, sequenceNumber=2, masterKeyId=2 on 172.31.10.82:8020
17/05/05 05:46:09 INFO security.TokenCache: Got dt for hdfs://ip-172-31-10-82.eu-central-1.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.10.82:8020, Ident: (token for jemaine: HDFS_DELEGATION_TOKEN owner=jemaine@MIHENN87.AU, renewer=yarn, realUser=, issueDate=1493977569868, maxDate=1494582369868, sequenceNumber=2, masterKeyId=2)
17/05/05 05:46:10 INFO input.FileInputFormat: Total input paths to process : 4
17/05/05 05:46:10 INFO mapreduce.JobSubmitter: number of splits:4
17/05/05 05:46:10 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493976890859_0002
17/05/05 05:46:10 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.10.82:8020, Ident: (token for jemaine: HDFS_DELEGATION_TOKEN owner=jemaine@MIHENN87.AU, renewer=yarn, realUser=, issueDate=1493977569868, maxDate=1494582369868, sequenceNumber=2, masterKeyId=2)
17/05/05 05:46:11 INFO impl.YarnClientImpl: Submitted application application_1493976890859_0002
17/05/05 05:46:11 INFO mapreduce.Job: The url to track the job: http://ip-172-31-10-82.eu-central-1.compute.internal:8088/proxy/application_1493976890859_0002/
17/05/05 05:46:11 INFO mapreduce.Job: Running job: job_1493976890859_0002
17/05/05 05:46:21 INFO mapreduce.Job: Job job_1493976890859_0002 running in uber mode : false
17/05/05 05:46:21 INFO mapreduce.Job:  map 0% reduce 0%
17/05/05 05:46:34 INFO mapreduce.Job:  map 25% reduce 0%
17/05/05 05:46:35 INFO mapreduce.Job:  map 50% reduce 0%
17/05/05 05:46:36 INFO mapreduce.Job:  map 75% reduce 0%
17/05/05 05:46:37 INFO mapreduce.Job:  map 100% reduce 0%
17/05/05 05:46:46 INFO mapreduce.Job:  map 100% reduce 100%
17/05/05 05:46:48 INFO mapreduce.Job: Job job_1493976890859_0002 completed successfully
17/05/05 05:46:48 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=65
                FILE: Number of bytes written=632286
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1212
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=19
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=4
                Launched reduce tasks=1
                Data-local map tasks=4
                Total time spent by all maps in occupied slots (ms)=24359
                Total time spent by all reduces in occupied slots (ms)=3527
                Total time spent by all map tasks (ms)=24359
                Total time spent by all reduce tasks (ms)=3527
                Total vcore-seconds taken by all map tasks=24359
                Total vcore-seconds taken by all reduce tasks=3527
                Total megabyte-seconds taken by all map tasks=24943616
                Total megabyte-seconds taken by all reduce tasks=3611648
        Map-Reduce Framework
                Map input records=4
                Map output records=8
                Map output bytes=72
                Map output materialized bytes=136
                Input split bytes=740
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=136
                Reduce input records=8
                Reduce output records=0
                Spilled Records=16
                Shuffled Maps =4
                Failed Shuffles=0
                Merged Map outputs=4
                GC time elapsed (ms)=132
                CPU time spent (ms)=3360
                Physical memory (bytes) snapshot=2046689280
                Virtual memory (bytes) snapshot=7942074368
                Total committed heap usage (bytes)=2284322816
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=472
        File Output Format Counters
                Bytes Written=97
Job Finished in 38.582 seconds
Estimated value of Pi is 3.13500000000000000000
[jemaine@ip-172-31-9-185 root]$
```