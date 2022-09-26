# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 7 Errata
<br>

If you run into issues pasting into the lab from the instructions - paste into notepad on the VM then into PowerShell<br>

<br>

## Module 07 (CSS): Migrating Hyper-V VMs to Azure by using Azure Migrate

<br>

### Exercise 1: Prepare the lab environment

<br>

Task 2: Deploy Azure Bastion<br>
Step 3: Copy and Paste does not work.  Will have to copy and paste manually.  You can copy all the lines at one time and paste at 1 time.  Hit enter with the last line appears<br>

Task 3: Deploy a nested VM in the Azure VM<br>
Do not even bother trying to connect with the Bastion, do the work around listed at the beginning of the lab.  Make sure you launch Bash not PowerShell and the commands have to be manually pasted.  Copy and paste and execute each group all at once<br>
Accept the default when Edge launches to get past the welcome screens.<br>
Step 6:  The .VHD will download into the downloads folder.  Move it to f:\VHDs folder<br>
Step 23: Command must be typed in manually<br>

<br>

### Exercise 2: Prepare for assessment and migration by using Azure Migrate


<br>

Task 1: Configure Hyper-V environment<br>
Step 3: Copy and paste in the upper pane of the PowerShell ISE, then click run<br>
Step 4: N is only selected for the 2 prompts when asked that are identified in the lab instructions, all others are Y<br>

<br>

### Exercise 3: Assess Hyper-V for migration by using Azure Migrate

<br>

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

<br>
