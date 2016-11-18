hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar pi 16 1000

Job Finished in 66.555 seconds

Estimated value of Pi is 3.14250000000000000000







[saxony@ip-172-31-6-143 root]$  hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar pi 16 1000
Number of Maps  = 16
Samples per Map = 1000
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Starting Job
16/11/18 14:43:50 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-6-142.us-west-2.compute.internal/172.31.6.142:8032
16/11/18 14:43:50 INFO hdfs.DFSClient: Created token for saxony: HDFS_DELEGATION_TOKEN owner=saxony@SKIRITI.IN, renewer=yarn, realUser=, issueDate=1479498230263, maxDate=1480103030263, sequenceNumber=2, masterKeyId=2 on 172.31.6.142:8020
16/11/18 14:43:50 INFO security.TokenCache: Got dt for hdfs://ip-172-31-6-142.us-west-2.compute.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.6.142:8020, Ident: (token for saxony: HDFS_DELEGATION_TOKEN owner=saxony@SKIRITI.IN, renewer=yarn, realUser=, issueDate=1479498230263, maxDate=1480103030263, sequenceNumber=2, masterKeyId=2)
16/11/18 14:43:50 INFO input.FileInputFormat: Total input paths to process : 16
16/11/18 14:43:50 INFO mapreduce.JobSubmitter: number of splits:16
16/11/18 14:43:50 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1479497415941_0002
16/11/18 14:43:50 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.6.142:8020, Ident: (token for saxony: HDFS_DELEGATION_TOKEN owner=saxony@SKIRITI.IN, renewer=yarn, realUser=, issueDate=1479498230263, maxDate=1480103030263, sequenceNumber=2, masterKeyId=2)
16/11/18 14:43:51 INFO impl.YarnClientImpl: Submitted application application_1479497415941_0002
16/11/18 14:43:51 INFO mapreduce.Job: The url to track the job: http://ip-172-31-6-142.us-west-2.compute.internal:8088/proxy/application_1479497415941_0002/
16/11/18 14:43:51 INFO mapreduce.Job: Running job: job_1479497415941_0002
16/11/18 14:44:22 INFO mapreduce.Job: Job job_1479497415941_0002 running in uber mode : false
16/11/18 14:44:22 INFO mapreduce.Job:  map 0% reduce 0%
16/11/18 14:44:32 INFO mapreduce.Job:  map 13% reduce 0%
16/11/18 14:44:38 INFO mapreduce.Job:  map 25% reduce 0%
16/11/18 14:44:39 INFO mapreduce.Job:  map 50% reduce 0%
16/11/18 14:44:41 INFO mapreduce.Job:  map 56% reduce 0%
16/11/18 14:44:45 INFO mapreduce.Job:  map 69% reduce 0%
16/11/18 14:44:47 INFO mapreduce.Job:  map 81% reduce 0%
16/11/18 14:44:48 INFO mapreduce.Job:  map 100% reduce 0%
16/11/18 14:44:56 INFO mapreduce.Job:  map 100% reduce 100%
16/11/18 14:44:56 INFO mapreduce.Job: Job job_1479497415941_0002 completed successfully
16/11/18 14:44:56 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=124
		FILE: Number of bytes written=2058214
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=4790
		HDFS: Number of bytes written=215
		HDFS: Number of read operations=67
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Job Counters 
		Launched map tasks=16
		Launched reduce tasks=1
		Data-local map tasks=16
		Total time spent by all maps in occupied slots (ms)=129104
		Total time spent by all reduces in occupied slots (ms)=6141
		Total time spent by all map tasks (ms)=129104
		Total time spent by all reduce tasks (ms)=6141
		Total vcore-seconds taken by all map tasks=129104
		Total vcore-seconds taken by all reduce tasks=6141
		Total megabyte-seconds taken by all map tasks=132202496
		Total megabyte-seconds taken by all reduce tasks=6288384
	Map-Reduce Framework
		Map input records=16
		Map output records=32
		Map output bytes=288
		Map output materialized bytes=544
		Input split bytes=2902
		Combine input records=0
		Combine output records=0
		Reduce input groups=2
		Reduce shuffle bytes=544
		Reduce input records=32
		Reduce output records=0
		Spilled Records=64
		Shuffled Maps =16
		Failed Shuffles=0
		Merged Map outputs=16
		GC time elapsed (ms)=915
		CPU time spent (ms)=10460
		Physical memory (bytes) snapshot=7601770496
		Virtual memory (bytes) snapshot=26694762496
		Total committed heap usage (bytes)=8689549312
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=1888
	File Output Format Counters 
		Bytes Written=97
Job Finished in 66.555 seconds
Estimated value of Pi is 3.14250000000000000000
