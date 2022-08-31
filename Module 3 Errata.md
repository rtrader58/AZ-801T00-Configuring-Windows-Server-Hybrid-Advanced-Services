# AZ-800T00 Configuring Windows Server  Hybrid Advanced Service - Module 3 Errata

## Module 3 Lab:  Implementing Failover Clustering

<br>

After downloading the lab files logon to SEA-SVR2 and restart the server<br>
While SEA-SVR2 is restarting logon to SEA-SVR1 and restart. Using PowerShell type restart-computer -force<br>

<br>

### Exercise 1: Configuring iSCSI storage

<br>

All the PowerShell commands need to copied and ran 1 at a time, do not paste multiple commands at a time.<br>
Example Exercise 1 > Task 1 > Step 3<br>

<br>

### In Task 1, 2 and 3 you will have 3 PowerShell windows open.  One connected to SEA-SVR2, one to SEA-DC1 and one to SEA-SVR1.  When running the commands make sure you are in the correct PowerShell window

<br>

### Exercise 2: Configuring a failover cluster

<br>

Task 1: Connect clients to the iSCSI targets<br>
Replace Step 1 with the following<br>
On SEA-SVR2. Navigate to Server Manager > File and Storage Services > iSCSI
Right click on the first disk > click Assign iScsi Virtual disk… > Click Next > Click Assign > Click Close – repeat this step for the 2 remaining disks<br>

Task 2: Initialize the disks<br>
Step 1: Take note of the drive numbers as they will not match the lab steps.<br>
The drives you just add will be drives 2, 3 and 4.  You will need to modify the PowerShell commands in the next step to match the correct drive number
Change the following PowerShell commands as follows:<br>
New-Partition -DiskNumber 1 -Size 5gb -AssignDriveLetter Change the disk number from 1 to 2<br>
New-Partition -DiskNumber 2 -Size 5gb -AssignDriveLetter Change the disk number from 2 to 3<br>
New-Partition -DiskNumber 3 -Size 5gb -AssignDriveLetter Change the disk number from 3 to 4<br>
