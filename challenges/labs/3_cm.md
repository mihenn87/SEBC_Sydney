# Userdirs
---
```bash
[hdfs@ip-172-31-10-82 root]$ hdfs dfs -ls /user
Found 7 items
drwxr-xr-x   - cate    cate             0 2017-05-05 04:48 /user/cate
drwxrwxrwx   - mapred  hadoop           0 2017-05-05 04:44 /user/history
drwxrwxr-t   - hive    hive             0 2017-05-05 04:44 /user/hive
drwxrwxr-x   - hue     hue              0 2017-05-05 04:45 /user/hue
drwxrwxr-x   - impala  impala           0 2017-05-05 04:45 /user/impala
drwxr-xr-x   - jemaine jemaine          0 2017-05-05 04:49 /user/jemaine
drwxrwxr-x   - oozie   oozie  
```

#API Hosts
```bash
[hdfs@ip-172-31-10-82 root]$ curl -u 'admin:sydney' 'http://localhost:7180/api/v14/hosts'
{
  "items" : [ {
    "hostId" : "21c6f1d3-6e5d-42bb-92ba-34505cab23bb",
    "ipAddress" : "172.31.10.82",
    "hostname" : "ip-172-31-10-82.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/hostRedirect/21c6f1d3-6e5d-42bb-92ba-34505cab23bb",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "a17633a9-27df-4651-8564-39442276c8c8",
    "ipAddress" : "172.31.13.251",
    "hostname" : "ip-172-31-13-251.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/hostRedirect/a17633a9-27df-4651-8564-39442276c8c8",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "41af6969-12ad-4688-8a94-2fa29fb3a397",
    "ipAddress" : "172.31.15.57",
    "hostname" : "ip-172-31-15-57.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/hostRedirect/41af6969-12ad-4688-8a94-2fa29fb3a397",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "8c9b175d-f994-4131-80b2-c080ae83de9a",
    "ipAddress" : "172.31.2.37",
    "hostname" : "ip-172-31-2-37.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/hostRedirect/8c9b175d-f994-4131-80b2-c080ae83de9a",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "daf9775c-4d6f-4c22-a67e-058331f93050",
    "ipAddress" : "172.31.9.185",
    "hostname" : "ip-172-31-9-185.eu-central-1.compute.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/hostRedirect/daf9775c-4d6f-4c22-a67e-058331f93050",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  } ]
 }

```

#API Services
```bash
[hdfs@ip-172-31-10-82 root]$ curl -u 'admin:sydney' 'http://localhost:7180/api/v6/clusters/mihenn87/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hive",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/zookeeper",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/oozie",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "impala",
    "type" : "IMPALA",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/impala",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "IMPALA_ASSIGNMENT_LOCALITY",
      "summary" : "DISABLED"
    }, {
      "name" : "IMPALA_CATALOGSERVER_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "IMPALA_IMPALADS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "IMPALA_STATESTORE_HEALTH",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Impala"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-10-82.eu-central-1.compute.internal:7180/cmf/serviceRedirect/hdfs",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS"
  } ]
}

```



