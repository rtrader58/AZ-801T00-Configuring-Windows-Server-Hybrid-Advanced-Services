# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 7 Errata

If you run into issues pasting into the lab from the instructions - open and paste into the PowerShell ISE <br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>

## Module 07 (CSS): Migrating Hyper-V VMs to Azure by using Azure Migrate

### Exercise 1: Prepare the lab environment

Task 1: Deploy an Azure VM by using an Azure Resource Manager QuickStart template<br>
Step 4: Use East US for region<br>
Step 5: The deployment took 25 minutes for me <br>

Task 2: Provide remote access<br>
Step 1: Does not paste into the lab browser - in a new lab browser tab type http://whatismyipaddress.com <br>
Step 3: Select no storage account needed > select your subscription > select Apply <br>
Step 4: Paste the last bash command into notepad and replace the WHATS-MY-IP-ADDRESS with the IP address obtained in step 1.  Then copy and paste into the cloudshell <br>

Task 3: Deploy a nested VM in the Azure VM<br>
Step 7: Follow the prompts to start Edge without data sync <br>
Step 7: Use the following link to download the .vhd - https://info.microsoft.com/ww-landing-windows-server-2022.html <br>
Step 7: Click VHD download, download will take ~8-10 minutes then copy will take ~5-8 minutes <br>
Step 23: If prompted to log in with HLKAdminUser click cancel to log on with the Administrator account <br>
Step 24: Use PowerShell ISE not PowerShell<br>

### Exercise 2: Prepare for assessment and migration by using Azure Migrate

Task 1: Configure Hyper-V environment<br>
Step 4: N is only selected for the 2 prompts when asked that are identified in the lab instructions, all others are Y<br>

### Exercise 3: Assess Hyper-V for migration by using Azure Migrate

Task 1: Deploy and configure the Azure Migrate appliance<br>
Step 2: Select All Projects > select az801lab07a-migrate-project <br>
Step 3: Select Start discovery > Using Appliance > for Azure <br>

Before starting the Task open Notepad in the RDP session copy and paste your Azure tenant credentials<br>
Step 4: Copy and paste the key in notepad in the RDP session<br>
Step 6: Move the .ZIP file to F:VMs<br>
Step 24: You cannot copy and paste from inside environment.  Open another tab in the Edge browser in AZ801l07a-vma1 and log into your Azure Portal<br>.   
Navigate to Azure Migrate > Servers, databases and web apps > Discover <br> 
Use the drop down box to select Yes, with Hyper-V.  Click Manager existing appliances.  Copy project key.  You will now be able to paste it in your appliance > select Verify<br>
If after step 29: Start Discovery is not available, ensure the slider under step 3 is set to the left<br>

Task 2: Configure, run, and view an assessment<br>
Step 2: Assessment settings not properties<br>
