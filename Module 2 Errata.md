# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 2 Errata

If you run into issues pasting into the lab from the instructions - open PowerShell ISE paste into PowerShell ISE<br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>

## Module 2 Implementing Security Solutions in a Hybrid Scenarios

### Exercise 1: Creating an Azure Log Analytics workspace and an Azure Automation account

Step 4: Resource group has already been created <br>

### Exercise 2: Configuring Microsoft Defender for Cloud

Skip - Task 1: Enable Defender for Cloud and automatic agent installation <br>

Task 2: Enable enhanced security of Defender for Cloud <br>
Step 13: Enabling the Sever took over 5 minutes <br>

### Exercise 3: Provisioning Azure VMs running Windows Server

Task 2: Deploy an Azure VM by using an Azure Resource Manager template<br>
Skip - Step 1: Resource group has already been created <br>
Step 6:  I used the Localadmin for user and password for the labuser account located in the Resources tab<br>

### Exercise 4: Onboarding on-premises Windows Server into Microsoft Defender for Cloud and Azure Automation

Task 1: Install Azure Arc agents on an On-Premises Server<br>
Step 2: In the navigation pane under All Azure Arc resources, Infrastructure, select Machines<br>
Step 3: Select + Onboard/Create, and in the dropdown, select Onboard existing machines<br>
Step 4: Under the Basic tab fill in the following information, Resource Group - AZ801-L0202-RG, Region - East US, leave the remaining setting as they are <br>
Skip steps 5 - 8<br>
Step 9: In the Onboard existing machines with Azure Arc tab, scroll down and select the Download and run script button, click Download on the page, select keep if prompted<br>
Step 10: Click on the Start menu and then right click on PowerShell ISE not PowerShell Prompt<br>
Step 11 - 15:  Paste inside of the PowerShell Prompt area inside the ISE. the script took 8 - 10 minutes to complete <br>
Step 17: Close the Onboard existing machines with Azure Arc page and navigate back to the Azure Arc Machines page<br>

Task 2: Enable Change Tracking and Inventory on the Arc machine<br>
Step 3: Wait for the deployment of the Change Tracking feature to complete, do not proceed as the instuctions say<br>

Task 3: Enable Monitoring using Insights<br>
Step 2: Under Monitoring select Insights, select Configure, remove checkmark for Preview OpenTelemetry metricsm and select Review + enable, select enable<br>
Skip steps 3 - 8: Data collection rule is already created, refresh the screen a couple of times you will see data being collected<br>

Task 5: Verify Azure Policy compliance, change tracking, Inventory, Insights monitoring, and Azure Updates<br>
Step 2: On the Get Started tab, select Analyze data. You should be able to see the performance data<br>
Step 3: I was not able to get any data on the Map tab, as the tab is being depricated<br>

### Exercise 5: Verifying the hybrid capabilities of Microsoft Defender for Cloud and Azure Automation solutions

No Errata<br>
