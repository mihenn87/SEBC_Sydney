#yum.repos.d

```
[root@ip-172-31-9-185 mysql-connector-java-5.1.41]# ls /etc/yum.repos.d
cloudera-manager.repo  redhat-rhui-client-config.repo
mariadb.repo           redhat-rhui.repo
redhat.repo            rhui-load-balancers.conf

```

#scm_prepare_database

```
/usr/share/cmf/schema/scm_prepare_database.sh mysql scm root cloudera
```
