---
title: "SCOM C Drive Disk Alerts"
date: 2023-02-26T14:14:54-05:00
authors:
  - Eric Lazar
---

Create a dynamic group of Logical Disk Objects like this:

![Scenario 1: Across columns](/dynamic-query-disk.png)

The Query formula then should look like this:

```( Object is Windows Server 2016 and above Logical Disk AND ( Device Name Equals C: ) AND True )```

<br>
For the Alert View, choose the dynamic group you created earlier.   You can also pick the object on the left to just be disks for a more efficient alert filter


![Scenario 1: Across columns](/scom-c-disk-alerts.png)