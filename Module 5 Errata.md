# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 5 Errata

## Keep an eye on the lab timer

If you run into issues pasting into the lab from the instructions - open PowerShell ISE paste into PowerShell ISE<br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>

## Module 05 (CSS): Implementing Azure-based recovery services

### Exercise 1: Creating and configuring an Azure Site Recovery vault

Task 1: Create an Azure Site Recovery vault<br>
Step 4: Use East US for the Region<br>

### Exercise 2: Implementing Hyper-V VM protection by using Azure Site Recovery vault

Task 1: Implement an Azure recovery site<br>
Step 3: Click Delete address space<br>
Step 11: Click Delete address space<br>

Task 2: Prepare protection of a Hyper-V virtual machine<br>
Step 2: Select Enable Site Recover<br>
Step 8:  Open the Group Policy Management console under Administrative Tools<br>
Step 11: Open Powershell ISE
Step 23: If unable to resolve to connect click try again<br>

Task 4: Review Azure VM replication settings<br>  
Step 2: Before proceeding to Step 3 wait for the Status to change to Synchronizing – took ~20 minutes then started synchronizing – then waiting for first recovery.  Once synchronization starts you can move to step 3<br>
Do not continue past Step 4 until Status changes to protected ~30 minutes from starting replication to getting Protected<br>

Task 5: Perform a failover of the Hyper-V virtual machine<br>
Step 3: Took ~4 minutes<br>
Step 5: Cleanup test failover is located on the top bar next to Test Failover<br>

### Exercise 4: Deprovisioning the Azure lab environment

Task 1: Remove the protected items<br>
Step 2 click on the sea-svr1 name to get to the next page.  You will have to use the scroll bar to scroll to the right at the bottom of the blade<br>

Task 2: Delete the lab resource groups<br>
Manually copy and paste the commands<br>
 
