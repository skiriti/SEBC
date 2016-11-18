time hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Ddfs.blocksize=16777216 51200000 tgen512m


real	1m8.130s
user	0m5.573s
sys	0m0.253s


hdfs dfs -ls /user/bavaria/tgen512m

Found 3 items

-rw-r--r--   3 bavaria supergroup          0 2016-11-18 14:08 /user/bavaria/tgen512m/_SUCCESS

-rw-r--r--   3 bavaria supergroup 2560000000 2016-11-18 14:08 /user/bavaria/tgen512m/part-m-00000

-rw-r--r--   3 bavaria supergroup 2560000000 2016-11-18 14:08 /user/bavaria/tgen512m/part-m-00001

hadoop fsck /user/bavaria/tgen512m

DEPRECATED: Use of this script to execute hdfs command is deprecated.

Instead use the hdfs command for it.

Connecting to namenode via http://ip-172-31-6-142.us-west-2.compute.internal:50070

FSCK started by bavaria (auth:SIMPLE) from /172.31.6.142 for path /user/bavaria/tgen512m at Fri Nov 18 14:10:17 EST 2016

...Status: HEALTHY

Total size:	5120000000 B

Total dirs:	1

Total files:	3

Total symlinks:		0


Total blocks (validated):	306 (avg. block size 16732026 B)

Minimally replicated blocks:	306 (100.0 %)

Over-replicated blocks:	0 (0.0 %)

Under-replicated blocks:	0 (0.0 %)

Mis-replicated blocks:		0 (0.0 %)

Default replication factor:	3

Average block replication:	3.0

Corrupt blocks:		0

Missing replicas:		0 (0.0 %)

Number of data-nodes:		4

Number of racks:		1

FSCK ended at Fri Nov 18 14:10:17 EST 2016 in 13 milliseconds



The filesystem under path '/user/bavaria/tgen512m' is HEALTHY
