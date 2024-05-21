# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 2 Errata

If you run into issues pasting into the lab from the instructions - open PowerShell ISE paste into PowerShell ISE<br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>

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
Skip Steps 16 and 17 they are no longer options in the Azure Portal <br>

### Exercise 3: Provisioning Azure VMs running Windows Server

Task 1: Start Azure Cloud Shell<br>
Step 2: on the Getting Started window select your subscription in the dropdown box  Click Apply<br>

Task 2: Deploy an Azure VM by using an Azure Resource Manager template<br>
Step 3: Paste each cmdlet into Notepad or the PowerShell ISE, in the first line replace '<azure_region>' with 'eastus' - then copy and paste from Notepad or the PowerShell ISE <br>

### Exercise 4: Onboarding on-premises Windows Server into Microsoft Defender for Cloud and Azure Automation

Task 1: Perform manual installation of the Log Analytics agent<br>
Step 5: Copy the Workspace ID and Primary Key and paste them into notepad<br>
Step 12:  If you did not close the Agent management blade in the Azure Portal you can copy and paste from the portal.  If you closed the blade copy and paste from notepad.  Must use Ctrl + V to paste<br>

Task 2: Perform unattended installation of the Log Analytics agent
Step 4:  Paste cmdlet into Notepad or the PowerShell ISE, in the replace "<WorkspaceID>" with "WorkspaceID copied in previous ste" and "<PrimaryKey>" with "PrimaryKey copied in previous ste" - then copy and paste from Notepad or the PowerShell ISE 

Task 2: Perform unattended installation of the Log Analytics agent<br>
Step 2: Copy and paste each command separately and press enter after pasting each, It may take up to 5 minutes before the threat is detected <br>

### Exercise 5: Verifying the hybrid capabilities of Microsoft Defender for Cloud and Azure Automation solutions

Task 2: Validate the threat detection capabilities for on-premises servers<br>
It may take up to 5-10 minutes before the threat is detected<br> 

Task 4: Validate Azure Automation solutions<br>
Step 7: On prem servers may not be listed, it took ~45 minutes for them to populate<br>
