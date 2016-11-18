[root@ip-172-31-6-142 temp]# mysql --version

mysql  Ver 14.14 Distrib 5.6.34, for Linux (x86_64) using  EditLine wrapper

mysql> show databases;

+--------------------+

| Database           |

+--------------------+

| information_schema |

| hive               |

| hue                |

| mysql              |

| oozie              |

| performance_schema |

| rman               |

| scm                |

| sentry             |

+--------------------+

9 rows in set (0.00 sec)

mysql> show grants;

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

| Grants for root@ip-172-31-6-142.us-west-2.compute.internal                                                                                                              |

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

| GRANT ALL PRIVILEGES ON *.* TO 'root'@'ip-172-31-6-142.us-west-2.compute.internal' IDENTIFIED BY PASSWORD '*81F5E21E35407D884A6CD4A731AEBFB6AF209E1B' WITH GRANT OPTION |

| GRANT PROXY ON ''@'' TO 'root'@'ip-172-31-6-142.us-west-2.compute.internal' WITH GRANT OPTION                                                                           |

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

2 rows in set (0.00 sec)

