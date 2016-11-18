mysql> show grants for root@'ip-172-31-6-143.us-west-2.compute.internal';

+----------------------------------------------------------------------------------------------------------------------------------------------+

| Grants for root@ip-172-31-6-143.us-west-2.compute.internal                                                                                   |

+----------------------------------------------------------------------------------------------------------------------------------------------+

| GRANT USAGE ON *.* TO 'root'@'ip-172-31-6-143.us-west-2.compute.internal' IDENTIFIED BY PASSWORD '*81F5E21E35407D884A6CD4A731AEBFB6AF209E1B' |

| GRANT ALL PRIVILEGES ON `rman`.* TO 'root'@'ip-172-31-6-143.us-west-2.compute.internal' WITH GRANT OPTION                                    |

| GRANT ALL PRIVILEGES ON `scm`.* TO 'root'@'ip-172-31-6-143.us-west-2.compute.internal' WITH GRANT OPTION                                     |

| GRANT ALL PRIVILEGES ON `hive`.* TO 'root'@'ip-172-31-6-143.us-west-2.compute.internal' WITH GRANT OPTION                                    |

+----------------------------------------------------------------------------------------------------------------------------------------------+

4 rows in set (0.00 sec)


[root@ip-172-31-6-142 temp]# hdfs dfs -ls /user/

Found 8 items

drwxr-xr-x   - admin   admin               0 2016-11-18 13:56 /user/admin

drwxr-xr-x   - bavaria supergroup          0 2016-11-18 13:54 /user/bavaria

drwxr-xr-x   - hdfs    supergroup          0 2016-11-18 13:56 /user/hdfs

drwxrwxrwx   - mapred  hadoop              0 2016-11-18 13:48 /user/history

drwxrwxr-t   - hive    hive                0 2016-11-18 13:49 /user/hive

drwxrwxr-x   - hue     hue                 0 2016-11-18 13:50 /user/hue

drwxrwxr-x   - oozie   oozie               0 2016-11-18 13:50 /user/oozie

drwxr-xr-x   - saxony  supergroup          0 2016-11-18 13:53 /user/saxony





{
  "items" : [ {
    "hostId" : "i-9d7eb133",
    "ipAddress" : "172.31.6.142",
    "hostname" : "ip-172-31-6-142.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-6-143.us-west-2.compute.internal:7180/cmf/hostRedirect/i-9d7eb133",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-9e7eb130",
    "ipAddress" : "172.31.6.143",
    "hostname" : "ip-172-31-6-143.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-6-143.us-west-2.compute.internal:7180/cmf/hostRedirect/i-9e7eb130",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-927eb13c",
    "ipAddress" : "172.31.6.144",
    "hostname" : "ip-172-31-6-144.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-6-143.us-west-2.compute.internal:7180/cmf/hostRedirect/i-927eb13c",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-937eb13d",
    "ipAddress" : "172.31.6.145",
    "hostname" : "ip-172-31-6-145.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-6-143.us-west-2.compute.internal:7180/cmf/hostRedirect/i-937eb13d",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "i-9c7eb132",
    "ipAddress" : "172.31.6.146",
    "hostname" : "ip-172-31-6-146.us-west-2.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-6-143.us-west-2.compute.internal:7180/cmf/hostRedirect/i-9c7eb132",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  } ]
}
