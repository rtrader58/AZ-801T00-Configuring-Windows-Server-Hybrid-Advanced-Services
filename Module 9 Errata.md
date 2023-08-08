# AZ-801T00 Configuring Windows Server  Hybrid Advanced Service - Module 9 Errata

If you run into issues pasting into the lab from the instructions - open PowerShell ISE paste into PowerShell ISE<br>
If using PowerShell run the command in PowerShell ISE <br>
If using the Azure Cloud Shell copy from the PowerShell ISE into the Cloud Shell <br>

## Note:  Throughout the lab the copy and paste shortcut in the lab may not work if you see ^V you will need to copy and paste manually

## Module 09 (CSS): Implementing operational monitoring in hybrid scenarios


### Exercise 1: Preparing a monitoring environment

Task 1: Deploy an Azure virtual machine<br>
Step 7: Paste each line individually manually – replace ‘<Azure_Region>’ with ‘eastus’<br>

### Exercise 2: Configuring monitoring of on-premises servers<br>

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
