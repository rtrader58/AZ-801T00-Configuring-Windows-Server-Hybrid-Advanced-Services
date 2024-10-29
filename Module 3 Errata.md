# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 3 Errata

If you run into issues pasting into the lab from the instructions - open PowerShell ISE paste into PowerShell ISE<br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>

## Module 3 Lab:  Implementing Failover Clustering

After downloading the lab files logon to SEA-SVR2 and restart the server<br>
While SEA-SVR2 is restarting logon to SEA-SVR1 and restart. Using PowerShell type restart-computer -force<br>

### Exercise 1: Configuring iSCSI storage

All the PowerShell commands need to copied pasted into the script block of the PowerShell ISE and then ran<br>

### In Task 1, 2 and 3 you will have 3 PowerShell ISE windows open.  One connected to SEA-SVR2, one to SEA-DC1 and one to SEA-SVR1.  When running the commands make sure you are in the correct PowerShell ISE window

### Exercise 2: Configuring a failover cluster

Task 2: Initialize the disks<br>
Step 1: Take note of the drive numbers as they may not match the lab steps.<br>
The drives you just add will need to be drives 2, 3 and 4.  You may need to modify the PowerShell commands in the next step to match the correct drive number
If needed, change the following PowerShell commands as follows:<br>
New-Partition -DiskNumber 1 -Size 5gb -AssignDriveLetter Change the disk number from 1 to 2<br>
New-Partition -DiskNumber 2 -Size 5gb -AssignDriveLetter Change the disk number from 2 to 3<br>
New-Partition -DiskNumber 3 -Size 5gb -AssignDriveLetter Change the disk number from 3 to 4<br>
