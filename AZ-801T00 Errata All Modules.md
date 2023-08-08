# AZ-801T00 Configuring Windows Server Hybrid Advanced Service - Errata All Modules

#  In all labs, if you run into issues pasting into the lab from the instructions - open PowerShell ISE and paste into PowerShell ISE instead of the PowerShell Prompt

## Module 1 Configuring security in Windows Server

### Exercise 1: Configuring Windows Defender Credential Guard

Task 2: Enable Windows Defender Credential Guard using the Hypervisor-Protected Code Integrity (HVCI) and Windows Defender Credential Guard hardware readiness tool<br>

Before doing the steps you will need to move C:\Allfiles\Labfiles to C:\Labfiles<br>

## Module 2 Implementing Security Solutions in a Hybrid Scenarios

### Exercise 1: Creating an Azure Log Analytics workspace and an Azure Automation account

Task 1: Create an Azure Log Analytics workspace<br>
Step 4: Choose East US for the Region<br>
Task 2: Create and configure an Azure Automation account<br>
Step 2: Choose East US 2 for the Region<br>

### Exercise 2: Configuring Microsoft Defender for Cloud

Task 2: Enable enhanced security of Defender for Cloud<br>
Step 6: If Log Analytics for Azure VMs is Off use the slide bar to turn it On<br>
Step 7: After choosing your Log Analytics Workspace select Exiting and new VMs<br>

### Exercise 3: Provisioning Azure VMs running Windows Server

Task 2: Deploy an Azure VM by using an Azure Resource Manager template<br>
Step 3: Copy and Paste each CMDLET separately<br>

### Exercise 4: Onboarding on-premises Windows Server into Microsoft Defender for Cloud and Azure Automation

Task 1: Perform manual installation of the Log Analytics agent<br>
Step 5: Copy the Workspace ID and Primary Key and paste them into notepadV
Step 12:  If you did not close the Agent management blade in the Azure Portal you can copy and paste from the portal.  If you closed the blade copy and paste from notepad.  Must use Ctrl + V to paste<br>

Task 2: Perform unattended installation of the Log Analytics agent<br>
Step 2: Copy and paste each command separately and press enter after pasting each
It may take up to 5 minutes before the threat is detected <br>

### Exercise 5: Verifying the hybrid capabilities of Microsoft Defender for Cloud and Azure Automation solutions

Task 2: Validate the threat detection capabilities for on-premises servers<br>
It may take up to 5-10 minutes before the threat is detected<br> 

Task 4: Validate Azure Automation solutions<br>
Step 7: On prem servers may not be listed, it took ~45 minutes for them to populate<br>
 
## Module 3 Lab:  Implementing Failover Clustering

After downloading the lab files logon to SEA-SVR2 and restart the server<br>
While SEA-SVR2 is restarting logon to SEA-SVR1 and restart. Using PowerShell type restart-computer -force<br>

### Exercise 1: Configuring iSCSI storage

All the PowerShell commands need to copied and ran 1 at a time, do not paste multiple commands at a time.<br>
Example Exercise 1 > Task 1 > Step 3<br>

### In Task 1, 2 and 3 you will have 3 PowerShell windows open.  One connected to SEA-SVR2, one to SEA-DC1 and one to SEA-SVR1.  When running the commands make sure you are in the correct PowerShell window

### Exercise 2: Configuring a failover cluster

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

## Module 04: Implementing Hyper-V Replica and Windows Server Backup

### Exercise1: Implementing Hyper-V Replica

Task 3: Validate a failover<br>
Step 6: You are not able to start the VM while it is replicating.  Move on to Exercise 2: Implementing backup and restore with Windows Server Backup – after completing come back and finish exercise 1 (My VM was still replicating – as long as you understand the concept you can end the lab if still replicating)
 
## Module 05 (CSS): Implementing Azure-based recovery services

<br>

### Exercise 1: Creating and configuring an Azure Site Recovery vault

Task 1: Create an Azure Site Recovery vault<br>
Step 4: Use East US for the Region<br>

### Exercise 2: Implementing Hyper-V VM protection by using Azure Site Recovery vault

Task 2: Prepare protection of a Hyper-V virtual machine<br>
Step 2: Select Enable Site Recover<br>

Task 4: Review Azure VM replication settings<br>
Step 2: Before proceeding to Step 3 wait for the Status to change to Synchronizing – took ~13 minutes then started synchronizing – then waiting for first recovery.  Once synchronization starts you can move to step 3<br>
Do not continue past Step 4 until Status changes to protected ~25 minutes from starting replication to getting Protected<br>

Task 5: Perform a failover of the Hyper-V virtual machine<br>
Step 3: Took ~4 minutes<br>
Step 5: Cleanup test failover is located on the top bar next to Test Failover<br>

### Exercise 4: Deprovisioning the Azure lab environment

Task 1: Remove the protected items<br>
Step 2 click on the sea-svr1 name to get to the next page.  You will have to use the scroll bar to scroll to the right at the bottom of the blade<br>

Task 2: Delete the lab resource groups<br>
Manually copy and paste the commands<br>
 
## Module 06 (CSS): Upgrade and migrate in Windows Server

### Exercise 1: Deploying AD DS domain controllers in Azure

Task 2: Deploy Azure Bastion<br>
Step 3: Copy and paste the commands manually<br>

Task 4: Manually promote a domain controller in an Azure VM<br>
Copy and Paste may not work while connected to az80106a-dc2, you may have to accomplish the steps manually<br>
Step 15: You may have to refresh Server Manager<br>

## Module 07 (CSS): Migrating Hyper-V VMs to Azure by using Azure Migrate

### Exercise 1: Prepare the lab environment

Task 2: Deploy Azure Bastion<br>
Step 3: Copy and Paste does not work.  Will have to copy and paste manually.  You can copy all the lines at one time and paste at 1 time.  Hit enter with the last line appears<br>

Task 3: Deploy a nested VM in the Azure VM<br>
Do not even bother trying to connect with the Bastion, do the work around listed at the beginning of the lab.  Make sure you launch Bash not PowerShell and the commands have to be manually pasted.  Copy and paste and execute each group all at once<br>
Accept the default when Edge launches to get past the welcome screens.<br>
Step 6:  The .VHD will download into the downloads folder.  Move it to f:\VHDs folder<br>
Step 23: Command must be typed in manually<br>

### Exercise 2: Prepare for assessment and migration by using Azure Migrate

Task 1: Configure Hyper-V environment<br>
Step 3: Copy and paste in the upper pane of the PowerShell ISE, then click run<br>
Step 4: N is only selected for the 2 prompts when asked that are identified in the lab instructions, all others are Y<br>

### Exercise 3: Assess Hyper-V for migration by using Azure Migrate

Task 1: Deploy and configure the Azure Migrate appliance<br>
Before starting the Task open Notepad in the RDP session copy and paste your Azure tenant credentials<br>
Step 4: Copy and paste the key in notepad in the RDP session<br>
Step 6: Move the .ZIP file to F:VMs<br>
Step 24: You cannot copy and paste from inside environment.  Open another tab in the Edge browser in AZ801l07a-vma1 and log into your Azure Portal<br>.   
Navigate to Azure Migrate > Servers, databases and web apps > Discover <br> 
Use the drop down box to select Yes, with Hyper-V.  Click Manager existing appliances.  Copy project key.  You will now be able to paste it in your appliance > select Verify<br>
If after step 29: Start Discovery is not available, ensure the slider under step 3 is set to the left<br>

Task 2: Configure, run, and view an assessment<br>
Step 2: Assessment settings not properties<br>

## Module 08: Monitoring and troubleshooting Windows Server

### No Errata

## Module 09 (CSS): Implementing operational monitoring in hybrid scenarios
## Note:  Throughout the lab the copy and paste shortcut in the lab may not work if you see ^V you will need to copy and paste manually

### Exercise 1: Preparing a monitoring environment

Task 1: Deploy an Azure virtual machine<br>
Step 7: Paste each line individually manually – replace ‘<Azure_Region>’ with ‘eastus’<br>
Exercise 2: Configuring monitoring of on-premises servers<br>

Task 1: Register Windows Admin Center with Azure<br>
NOTE:  The Windows Admin Center is preinstalled – skip to step 4<br>
Step 16:  If Sign in fail close the dialog box and on the Account page click Sign in and then select Accept<br>
Step 17; Browse back to the Windows Admin Center. There is a shortcut on the Edge task bar<br>

Task 2: Integrate an on-premises Windows Server with Azure Monitor<br>
Step 3: Click Set up<br>
Step 4: Use existing Resources Group<br>

### Exercise 3: Configuring monitoring of Azure VMs

Task 2: Configure diagnostic settings and VM Insights<br>
Skip step 4 as guest log diagnostic are already enabled<br>
Step 13: Enable Identity Management and click save.  Browse back to the VM diagnostics blade.  Refresh the browser.<br>
Step 21 and 22:  If Try now is not available, they are already enabled<br>
Step 23, in the Monitor | Virtual Machines page click on Workspace configuration in the middle of the screen<br>

### Exercise 4: Evaluating monitoring services

Task 1: Review Azure Monitor monitoring and alerting functionality<br>
Step 5: Click on New Alert Rule<br>
Step 14: Wait 10 minutes before proceeding<br>
