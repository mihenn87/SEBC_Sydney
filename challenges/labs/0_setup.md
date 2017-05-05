#Preperation
---

```bash

[root@ip-172-31-9-185 ec2-user]# sysctl -w vm.swappiness=1
vm.swappiness = 1
[root@ip-172-31-9-185 ec2-user]# echo 'never' > defrag_file_pathname
[root@ip-172-31-9-185 ec2-user]#


```

#Setup
---

##Cloudprovider
AWS

##Nodes

|external hostname	|ext. IP		|internal hostname	|int. IP|
|---|---|---|---|
|ec2-52-59-254-107.eu-central-1.compute.amazonaws.com	|52.59.254.107		|ip-172-31-10-82.eu-central-1.compute.internal	|172.31.10.82|
|ec2-54-93-252-216.eu-central-1.compute.amazonaws.com	|54.93.252.216		|ip-172-31-9-185.eu-central-1.compute.internal	|172.31.9.185|
|ec2-52-59-205-142.eu-central-1.compute.amazonaws.com	|52.59.205.142		|ip-172-31-2-37.eu-central-1.compute.internal	|172.31.2.37|
|ec2-52-59-252-4.eu-central-1.compute.amazonaws.com	|52.59.252.4		|ip-172-31-13-251.eu-central-1.compute.internal	|172.31.13.251|
|ec2-54-93-230-126.eu-central-1.compute.amazonaws.com	|54.93.230.126		|ip-172-31-15-57.eu-central-1.compute.internal	|172.31.15.57|

##Linux Release

```bash
[root@ip-172-31-2-37 ec2-user]# cat /etc/*-release
NAME="Red Hat Enterprise Linux Server"
VERSION="7.2 (Maipo)"
ID="rhel"
ID_LIKE="fedora"
VERSION_ID="7.2"
PRETTY_NAME="Red Hat Enterprise Linux Server 7.2 (Maipo)"
ANSI_COLOR="0;31"
CPE_NAME="cpe:/o:redhat:enterprise_linux:7.2:GA:server"
HOME_URL="https://www.redhat.com/"
BUG_REPORT_URL="https://bugzilla.redhat.com/"

REDHAT_BUGZILLA_PRODUCT="Red Hat Enterprise Linux 7"
REDHAT_BUGZILLA_PRODUCT_VERSION=7.2
REDHAT_SUPPORT_PRODUCT="Red Hat Enterprise Linux"
REDHAT_SUPPORT_PRODUCT_VERSION="7.2"
Red Hat Enterprise Linux Server release 7.2 (Maipo)
Red Hat Enterprise Linux Server release 7.2 (Maipo)

```

##Diskcapacity
```bash
[root@ip-172-31-2-37 ec2-user]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       30G  927M   30G   4% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   17M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000

```

##Repolist
```bash
[root@ip-172-31-9-185 ec2-user]# yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
rhui-REGION-client-config-server-7                      | 2.9 kB     00:00
rhui-REGION-rhel-server-releases                        | 3.5 kB     00:00
rhui-REGION-rhel-server-rh-common                       | 3.8 kB     00:00
(1/7): rhui-REGION-rhel-server-releases/7Server/x86_64/gr | 701 kB   00:00
(2/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/g |  104 B   00:00
(3/7): rhui-REGION-rhel-server-releases/7Server/x86_64/up | 1.9 MB   00:00
(4/7): rhui-REGION-client-config-server-7/x86_64/primary_ | 4.3 kB   00:00
(5/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/p | 118 kB   00:00
(6/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/u |  33 kB   00:00
(7/7): rhui-REGION-rhel-server-releases/7Server/x86_64/pr |  35 MB   00:00
repo id                                          repo name               status
rhui-REGION-client-config-server-7/x86_64        Red Hat Update Infrastr      4
rhui-REGION-rhel-server-releases/7Server/x86_64  Red Hat Enterprise Linu 14,277
rhui-REGION-rhel-server-rh-common/7Server/x86_64 Red Hat Enterprise Linu    228
repolist: 14,509
```

##User and Gropus

```bash
[root@ip-172-31-9-185 ec2-user]# groupadd kiwis
[root@ip-172-31-9-185 ec2-user]# groupadd aussies
[root@ip-172-31-9-185 ec2-user]# useradd -u 2300 -g aussies cate
[root@ip-172-31-9-185 ec2-user]# useradd -u 2900 -g kiwis jemaine
[root@ip-172-31-9-185 ec2-user]# cat /etc/passwd | grep cate
cate:x:2300:1002::/home/cate:/bin/bash
[root@ip-172-31-9-185 ec2-user]# cat /etc/passwd | grep jemaine
jemaine:x:2900:1001::/home/jemaine:/bin/bash
[root@ip-172-31-9-185 ec2-user]# cat /etc/group | grep kiwis
kiwis:x:1001:
[root@ip-172-31-9-185 ec2-user]# cat /etc/group | grep aussies
aussies:x:1002:
```