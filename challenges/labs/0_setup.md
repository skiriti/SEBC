region  : US West (Oregon)

AMI ID  : RHEL-7.2_HVM_GA-20151112-x86_64-1-Hourly2-GP2 (ami-775e4f16

OS      : RHEL - 7.2

Volume Space is : 80GB


[ec2-user@ip-172-31-6-142 ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       80G  928M   80G   2% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000


[ec2-user@ip-172-31-6-142 ~]$ yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-7.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-7.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Could not contact CDS load balancer rhui2-cds01.us-west-2.aws.ce.redhat.com, trying others.


Could not contact any CDS load balancers: rhui2-cds01.us-west-2.aws.ce.redhat.com, rhui2-cds02.us-west-2.aws.ce.redhat.com.



[root@ip-172-31-6-142 temp]# cat /etc/passwd | grep 'bavaria'

bavaria:x:2700:2700::/home/bavaria:/bin/bash

[root@ip-172-31-6-142 temp]# cat /etc/passwd | grep 'saxony'

saxony:x:2800:2800::/home/saxony:/bin/bash



root@ip-172-31-6-142 temp]# cat /etc/group | grep 'democratic'

democratic:x:2801:saxony

[root@ip-172-31-6-142 temp]# cat /etc/group | grep 'social'

social:x:2802:bavaria



