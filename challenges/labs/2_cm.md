[root@ip-172-31-6-143 yum.repos.d]# ls /etc/yum.repos.d

cloudera-manager.repo  mysql-community-source.repo  redhat-rhui-client-config.repo  rhui-load-balancers.conf

mysql-community.repo   redhat.repo                  redhat-rhui.repo


grant all on scm.* to 'root'@'%' with grant option;




/usr/share/cmf/schema/scm_prepare_database.sh mysql -h ip-172-31-6-142.us-west-2.compute.internal scm root root

JAVA_HOME=/usr/java/jdk1.8.0_60/jre/

Verifying that we can write to /etc/cloudera-scm-server

Creating SCM configuration file in /etc/cloudera-scm-server

Executing:  /usr/java/jdk1.8.0_60/jre//bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.

[                          main] DbCommandExecutor              INFO  Successfully connected to database.

All done, your SCM database is configured correctly!



