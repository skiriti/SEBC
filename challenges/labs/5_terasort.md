hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort tgen512m tsort512m


[bavaria@ip-172-31-6-142 temp]$ hdfs dfs -ls tsort512m

Found 10 items

-rw-r--r--   1 bavaria supergroup          0 2016-11-18 14:44 tsort512m/_SUCCESS

-rw-r--r--  10 bavaria supergroup         77 2016-11-18 14:39 tsort512m/_partition.lst

-rw-r--r--   1 bavaria supergroup  647943000 2016-11-18 14:44 tsort512m/part-r-00000

-rw-r--r--   1 bavaria supergroup  636583800 2016-11-18 14:44 tsort512m/part-r-00001

-rw-r--r--   1 bavaria supergroup  641196500 2016-11-18 14:44 tsort512m/part-r-00002


-rw-r--r--   1 bavaria supergroup  641695600 2016-11-18 14:44 tsort512m/part-r-00003

-rw-r--r--   1 bavaria supergroup  639210500 2016-11-18 14:44 tsort512m/part-r-00004

-rw-r--r--   1 bavaria supergroup  649849800 2016-11-18 14:44 tsort512m/part-r-00005

-rw-r--r--   1 bavaria supergroup  629886500 2016-11-18 14:44 tsort512m/part-r-00006

-rw-r--r--   1 bavaria supergroup  633634300 2016-11-18 14:44 tsort512m/part-r-00007









[bavaria@ip-172-31-6-142 temp]$ time hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort tgen512m tsort512m
16/11/18 14:39:50 INFO terasort.TeraSort: starting
16/11/18 14:39:51 INFO hdfs.DFSClient: Created token for bavaria: HDFS_DELEGATION_TOKEN owner=bavaria@SKIRITI.IN, renewer=yarn, realUser=, issueDate=1479497991886, maxDate=1480102791886, sequenceNumber=1, masterKeyId=2 on 172.31.6.142:8020
16/11/18 14:39:51 INFO security.TokenCache: Got dt for hdfs://ip-172-31-6-142.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.6.142:8020, Ident: (token for bavaria: HDFS_DELEGATION_TOKEN owner=bavaria@SKIRITI.IN, renewer=yarn, realUser=, issueDate=1479497991886, maxDate=1480102791886, sequenceNumber=1, masterKeyId=2)
16/11/18 14:39:52 INFO input.FileInputFormat: Total input paths to process : 2
Spent 403ms computing base-splits.
Spent 5ms computing TeraScheduler splits.
Computing input splits took 409ms
Sampling 10 splits of 306
Making 8 from 100000 sampled records
Computing parititions took 1171ms
Spent 1582ms computing partitions.
16/11/18 14:39:53 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-6-142.us-west-2.compute.internal/172.31.6.142:8032
16/11/18 14:39:53 INFO mapreduce.JobSubmitter: number of splits:306
16/11/18 14:39:53 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1479497415941_0001
16/11/18 14:39:53 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.6.142:8020, Ident: (token for bavaria: HDFS_DELEGATION_TOKEN owner=bavaria@SKIRITI.IN, renewer=yarn, realUser=, issueDate=1479497991886, maxDate=1480102791886, sequenceNumber=1, masterKeyId=2)
16/11/18 14:39:54 INFO impl.YarnClientImpl: Submitted application application_1479497415941_0001
16/11/18 14:39:54 INFO mapreduce.Job: The url to track the job: http://ip-172-31-6-142.us-west-2.compute.internal:8088/proxy/application_1479497415941_0001/
16/11/18 14:39:54 INFO mapreduce.Job: Running job: job_1479497415941_0001
16/11/18 14:40:04 INFO mapreduce.Job: Job job_1479497415941_0001 running in uber mode : false
16/11/18 14:40:04 INFO mapreduce.Job:  map 0% reduce 0%
16/11/18 14:40:15 INFO mapreduce.Job:  map 1% reduce 0%
16/11/18 14:40:23 INFO mapreduce.Job:  map 5% reduce 0%
16/11/18 14:40:25 INFO mapreduce.Job:  map 6% reduce 0%
16/11/18 14:40:35 INFO mapreduce.Job:  map 10% reduce 0%
16/11/18 14:40:36 INFO mapreduce.Job:  map 11% reduce 0%
16/11/18 14:40:45 INFO mapreduce.Job:  map 12% reduce 0%
16/11/18 14:40:46 INFO mapreduce.Job:  map 13% reduce 0%
16/11/18 14:40:47 INFO mapreduce.Job:  map 15% reduce 0%
16/11/18 14:40:48 INFO mapreduce.Job:  map 16% reduce 0%
16/11/18 14:40:56 INFO mapreduce.Job:  map 17% reduce 0%
16/11/18 14:40:58 INFO mapreduce.Job:  map 18% reduce 0%
16/11/18 14:41:00 INFO mapreduce.Job:  map 20% reduce 0%
16/11/18 14:41:02 INFO mapreduce.Job:  map 21% reduce 0%
16/11/18 14:41:05 INFO mapreduce.Job:  map 22% reduce 0%
16/11/18 14:41:08 INFO mapreduce.Job:  map 23% reduce 0%
16/11/18 14:41:11 INFO mapreduce.Job:  map 24% reduce 0%
16/11/18 14:41:12 INFO mapreduce.Job:  map 25% reduce 0%
16/11/18 14:41:14 INFO mapreduce.Job:  map 26% reduce 0%
16/11/18 14:41:15 INFO mapreduce.Job:  map 27% reduce 0%
16/11/18 14:41:21 INFO mapreduce.Job:  map 28% reduce 0%
16/11/18 14:41:22 INFO mapreduce.Job:  map 29% reduce 0%
16/11/18 14:41:23 INFO mapreduce.Job:  map 30% reduce 0%
16/11/18 14:41:24 INFO mapreduce.Job:  map 31% reduce 0%
16/11/18 14:41:28 INFO mapreduce.Job:  map 32% reduce 0%
16/11/18 14:41:31 INFO mapreduce.Job:  map 33% reduce 0%
16/11/18 14:41:33 INFO mapreduce.Job:  map 34% reduce 0%
16/11/18 14:41:36 INFO mapreduce.Job:  map 36% reduce 0%
16/11/18 14:41:41 INFO mapreduce.Job:  map 37% reduce 0%
16/11/18 14:41:42 INFO mapreduce.Job:  map 38% reduce 0%
16/11/18 14:41:43 INFO mapreduce.Job:  map 39% reduce 0%
16/11/18 14:41:47 INFO mapreduce.Job:  map 40% reduce 0%
16/11/18 14:41:48 INFO mapreduce.Job:  map 41% reduce 0%
16/11/18 14:41:51 INFO mapreduce.Job:  map 42% reduce 0%
16/11/18 14:41:52 INFO mapreduce.Job:  map 43% reduce 0%
16/11/18 14:41:54 INFO mapreduce.Job:  map 44% reduce 0%
16/11/18 14:41:58 INFO mapreduce.Job:  map 45% reduce 0%
16/11/18 14:42:00 INFO mapreduce.Job:  map 47% reduce 0%
16/11/18 14:42:03 INFO mapreduce.Job:  map 48% reduce 0%
16/11/18 14:42:04 INFO mapreduce.Job:  map 49% reduce 0%
16/11/18 14:42:09 INFO mapreduce.Job:  map 50% reduce 0%
16/11/18 14:42:12 INFO mapreduce.Job:  map 52% reduce 0%
16/11/18 14:42:13 INFO mapreduce.Job:  map 53% reduce 0%
16/11/18 14:42:15 INFO mapreduce.Job:  map 54% reduce 0%
16/11/18 14:42:18 INFO mapreduce.Job:  map 55% reduce 0%
16/11/18 14:42:21 INFO mapreduce.Job:  map 56% reduce 0%
16/11/18 14:42:24 INFO mapreduce.Job:  map 58% reduce 0%
16/11/18 14:42:26 INFO mapreduce.Job:  map 59% reduce 0%
16/11/18 14:42:27 INFO mapreduce.Job:  map 60% reduce 0%
16/11/18 14:42:36 INFO mapreduce.Job:  map 61% reduce 0%
16/11/18 14:42:37 INFO mapreduce.Job:  map 64% reduce 0%
16/11/18 14:42:38 INFO mapreduce.Job:  map 65% reduce 0%
16/11/18 14:42:46 INFO mapreduce.Job:  map 66% reduce 0%
16/11/18 14:42:47 INFO mapreduce.Job:  map 67% reduce 0%
16/11/18 14:42:49 INFO mapreduce.Job:  map 69% reduce 0%
16/11/18 14:42:50 INFO mapreduce.Job:  map 70% reduce 0%
16/11/18 14:42:55 INFO mapreduce.Job:  map 71% reduce 0%
16/11/18 14:42:57 INFO mapreduce.Job:  map 72% reduce 0%
16/11/18 14:42:59 INFO mapreduce.Job:  map 73% reduce 0%
16/11/18 14:43:00 INFO mapreduce.Job:  map 74% reduce 0%
16/11/18 14:43:02 INFO mapreduce.Job:  map 75% reduce 0%
16/11/18 14:43:04 INFO mapreduce.Job:  map 76% reduce 0%
16/11/18 14:43:10 INFO mapreduce.Job:  map 78% reduce 0%
16/11/18 14:43:12 INFO mapreduce.Job:  map 79% reduce 0%
16/11/18 14:43:13 INFO mapreduce.Job:  map 80% reduce 0%
16/11/18 14:43:15 INFO mapreduce.Job:  map 81% reduce 0%
16/11/18 14:43:21 INFO mapreduce.Job:  map 83% reduce 0%
16/11/18 14:43:22 INFO mapreduce.Job:  map 84% reduce 0%
16/11/18 14:43:23 INFO mapreduce.Job:  map 85% reduce 0%
16/11/18 14:43:28 INFO mapreduce.Job:  map 85% reduce 3%
16/11/18 14:43:29 INFO mapreduce.Job:  map 86% reduce 3%
16/11/18 14:43:31 INFO mapreduce.Job:  map 86% reduce 7%
16/11/18 14:43:35 INFO mapreduce.Job:  map 87% reduce 14%
16/11/18 14:43:36 INFO mapreduce.Job:  map 87% reduce 17%
16/11/18 14:43:37 INFO mapreduce.Job:  map 88% reduce 24%
16/11/18 14:43:39 INFO mapreduce.Job:  map 88% reduce 25%
16/11/18 14:43:42 INFO mapreduce.Job:  map 89% reduce 25%
16/11/18 14:43:43 INFO mapreduce.Job:  map 89% reduce 26%
16/11/18 14:43:45 INFO mapreduce.Job:  map 90% reduce 26%
16/11/18 14:43:48 INFO mapreduce.Job:  map 91% reduce 26%

16/11/18 14:43:52 INFO mapreduce.Job:  map 92% reduce 27%
16/11/18 14:43:55 INFO mapreduce.Job:  map 93% reduce 27%
16/11/18 14:44:00 INFO mapreduce.Job:  map 94% reduce 27%
16/11/18 14:44:02 INFO mapreduce.Job:  map 95% reduce 27%
16/11/18 14:44:03 INFO mapreduce.Job:  map 95% reduce 28%
16/11/18 14:44:06 INFO mapreduce.Job:  map 96% reduce 28%
16/11/18 14:44:10 INFO mapreduce.Job:  map 97% reduce 28%
16/11/18 14:44:11 INFO mapreduce.Job:  map 98% reduce 28%
16/11/18 14:44:13 INFO mapreduce.Job:  map 98% reduce 29%
16/11/18 14:44:16 INFO mapreduce.Job:  map 99% reduce 29%
16/11/18 14:44:19 INFO mapreduce.Job:  map 100% reduce 29%
16/11/18 14:44:21 INFO mapreduce.Job:  map 100% reduce 34%
16/11/18 14:44:22 INFO mapreduce.Job:  map 100% reduce 41%
16/11/18 14:44:23 INFO mapreduce.Job:  map 100% reduce 44%
16/11/18 14:44:24 INFO mapreduce.Job:  map 100% reduce 55%
16/11/18 14:44:25 INFO mapreduce.Job:  map 100% reduce 58%
16/11/18 14:44:26 INFO mapreduce.Job:  map 100% reduce 62%
16/11/18 14:44:27 INFO mapreduce.Job:  map 100% reduce 66%
16/11/18 14:44:29 INFO mapreduce.Job:  map 100% reduce 68%
16/11/18 14:44:30 INFO mapreduce.Job:  map 100% reduce 72%
16/11/18 14:44:32 INFO mapreduce.Job:  map 100% reduce 76%
16/11/18 14:44:33 INFO mapreduce.Job:  map 100% reduce 81%
16/11/18 14:44:35 INFO mapreduce.Job:  map 100% reduce 84%
16/11/18 14:44:36 INFO mapreduce.Job:  map 100% reduce 87%
16/11/18 14:44:38 INFO mapreduce.Job:  map 100% reduce 90%
16/11/18 14:44:39 INFO mapreduce.Job:  map 100% reduce 91%
16/11/18 14:44:41 INFO mapreduce.Job:  map 100% reduce 95%
16/11/18 14:44:42 INFO mapreduce.Job:  map 100% reduce 97%
16/11/18 14:44:43 INFO mapreduce.Job:  map 100% reduce 99%
16/11/18 14:44:44 INFO mapreduce.Job:  map 100% reduce 100%
16/11/18 14:44:45 INFO mapreduce.Job: Job job_1479497415941_0001 completed successfully
16/11/18 14:44:45 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=2268633901
		FILE: Number of bytes written=4528124610
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=5120047124
		HDFS: Number of bytes written=5120000000
		HDFS: Number of read operations=942
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters 
		Launched map tasks=306
		Launched reduce tasks=8
		Data-local map tasks=305
		Rack-local map tasks=1
		Total time spent by all maps in occupied slots (ms)=2862674
		Total time spent by all reduces in occupied slots (ms)=589000
		Total time spent by all map tasks (ms)=2862674
		Total time spent by all reduce tasks (ms)=589000
		Total vcore-seconds taken by all map tasks=2862674
		Total vcore-seconds taken by all reduce tasks=589000
		Total megabyte-seconds taken by all map tasks=2931378176
		Total megabyte-seconds taken by all reduce tasks=603136000
	Map-Reduce Framework
		Map input records=51200000
		Map output records=51200000
		Map output bytes=5222400000
		Map output materialized bytes=2221231103
		Input split bytes=47124
		Combine input records=0
		Combine output records=0
		Reduce input groups=51200000
		Reduce shuffle bytes=2221231103
		Reduce input records=51200000
		Reduce output records=51200000
		Spilled Records=102400000
		Shuffled Maps =2448
		Failed Shuffles=0
		Merged Map outputs=2448
		GC time elapsed (ms)=37636
		CPU time spent (ms)=1140910
		Physical memory (bytes) snapshot=154824318976
		Virtual memory (bytes) snapshot=494153641984
		Total committed heap usage (bytes)=176671948800
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=5120000000
	File Output Format Counters 
		Bytes Written=5120000000
16/11/18 14:44:45 INFO terasort.TeraSort: done

real	4m56.285s
user	0m9.166s
sys	0m0.339s


