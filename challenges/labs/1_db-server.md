##Hostname
```
MariaDB [(none)]> select @@hostname;
+-----------------------------------------------+
| @@hostname                                    |
+-----------------------------------------------+
| ip-172-31-10-82.eu-central-1.compute.internal |
+-----------------------------------------------+
1 row in set (0.00 sec)
```

##Version
```
MariaDB [(none)]> select @@version;
+----------------+
| @@version      |
+----------------+
| 5.5.56-MariaDB |
+----------------+
1 row in set (0.00 sec)
```

##Databases
```
MariaDB [(none)]> show databases;
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
```