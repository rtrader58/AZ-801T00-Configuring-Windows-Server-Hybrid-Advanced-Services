# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 7 Errata

If you run into issues pasting into the lab from the instructions - open and paste into the PowerShell ISE <br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>
The work around steps to bypass the Bastion have been integrated into Exercise 1 Task 2 of the lab <br>

## Module 07 (CSS): Migrating Hyper-V VMs to Azure by using Azure Migrate

### Exercise 1: Prepare the lab environment

Task 1: Deploy an Azure VM by using an Azure Resource Manager QuickStart template<br>
Step 4: Use East US for region<br>
Step 5: The deployment took ~25 minutes <br>

Task 2: Provide remote access<br>
Step 1: Does not paste into the lab browser - in a new lab browser tab type http://whatismyipaddress.com <br>
Step 3: Select no storage account needed > select your subscription > select Apply <br>
Step 4: Paste the last bash command into notepad and replace the WHATS-MY-IP-ADDRESS with the IP address obtained in step 1 leave the /32.  Then copy and paste into the cloudshell <br>

Task 3: Deploy a nested VM in the Azure VM<br>
Step 3: Open the downloaded RDP file, you may get disconnected on your initial connection, if so let it auto reconnect <br>
Step 7: Follow the prompts to start Edge without data sync <br>
Step 7: Use the following link to download the .vhd - https://info.microsoft.com/ww-landing-windows-server-2022.html <br>
Step 7: Click VHD download, download will take ~5-8 minutes then copy will take ~3-5 minutes <br>
Step 24: Use PowerShell ISE not PowerShell<br>

### Exercise 2: Prepare for assessment and migration by using Azure Migrate

Task 1: Configure Hyper-V environment<br>
Step 4: N is only selected for the 2 prompts when asked that are identified in the lab instructions, all others are Y<br>

Task 3: Implement the target Azure environment<br>
Step 19: When creating the storage account allow anonymous access on the Advanced tab<br>

### Exercise 3: Assess Hyper-V for migration by using Azure Migrate

Task 1: Deploy and configure the Azure Migrate appliance<br>
Before starting the Task open Notepad in the RDP session copy and paste your Azure tenant credentials<br>
Step 2: Select All Projects > select az801lab07a-migrate-project <br>
Step 3: Select Start discovery > Using Appliance > for Azure <br>
Step 5: Copy and paste the key in notepad in the RDP session<br>
Step 6: You will not be prompted, once downloaded move the .ZIP file to F:VMs<br>
Step 10: Browse to the F:\VMs <br>
Step 24: This step will take a while. You cannot copy and paste from dirctly inside environment.  In the menu of The VM click Clipboard > Type clipboard text <br>
Step 24: You have to wait run auto update status multiple times to complete, each time you will need to click Verifying.  Refresh may take a few moments after you click it.  Before you will be able to logon. Logon and registering took ~10 minutes, if the page times out, refresh the page.<br>
If after step 29: Start Discovery is not available, ensure the slider under step 3 is set to the left<br>
Step 30: Wait for the discovery to finish ~15-20 minutes <br>

Task 2: Configure, run, and view an assessment<br>
Replace steps 1 - 10 with the following <br>
Step 1: Expand Explore Inventory > Select All Inventory <br>
Step 2: Select the VM you want to Migrate > Select Create assessment <br>
Step 3: Basics Tab Use the name from step 6, select Review and create, Create <br>

Step 3: General Tab > configure the following: Region - East US, Default saving option - None, select Review and create, Create <br>
Step 4: Expand Decide and plan > Assessments > select the newly created assessment az801l07a-assessment <br>

### Exercise 4: Migrate Hyper-V VMs by using Azure Migrate

Task 1: Prepare for migration of Hyper-V VMs <br>
Replace Steps 1 - 2 with the following <br>
Step 1: Expand Execute > Migration > Discover more <br>
Step 13: Click Register before finishing <br>
Step 14 - 16: Refresh the Discover page > click Finalize registration - Wait for registration to complete ~15 minutes - Close button will be available <br>

Task 2: Configure replication of Hyper-V VMs <br>
Step 1: Expand Execute > Migrations > Replicate <br>
Step 3: There is no Assessment Group <br>
Step 10: Expand Execute > Migrations > Replication summary > Migration > Replications - click refresh > do not continue until the status shows protected <br>

Task 3: Perform migration of Hyper-V VMs <br>
Before continueing select Azure Home  <br>
Step 1: Navigate Azure Migrate > Expand Execute > Migrations > Replication summary > Migration > Replications <br>
Step 2: Click on ... select Test migration
Step 3: Click Refresh to update status - wait for status 





