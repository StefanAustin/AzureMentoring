### This lab is about Powershell and Azure

Powershell was a Microsoft command line but it is available on Linux. The following labs gives you ability to connect to Azure via Powershell.

### Installation instructions for other OS are here: 

https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-linux?view=powershell-7.1

If you use a Linux, the installation will take a while.

### First lab:
https://docs.microsoft.com/en-us/learn/modules/automate-azure-tasks-with-powershell/4-exercise-install-azure-powershell/

Do the page 5, to get powershell ready for use.

If you run into problems, use the command: Connect-AzAccount -UseDeviceAuthentication and open a browser https://microsoft.com/devicelogin and add the code.

- The module is somewhat messed up. The learning content asks you to select a subscription, but the next page will create a sandbox and if you use your subscription, you will get some errors.

https://docs.microsoft.com/en-us/learn/modules/automate-azure-tasks-with-powershell/6-exercise-create-resource-interactively/

If you used your subscription, you have to sign in and sign-out again to get the new learn resouce group.

Pick a long password to create the VM, like this one:
GGFDF55#$%a


The lab and the matching commands will delete the resources. Before you delete the VM, you can use the Azure Portal to see your VM.

## Tasks:
- Modify the create VM command and try to add a CentOs machine. Think about the parameters, you have to change two things.
You need to find a valid image name. CentOS will work, but you can look for others.

- You can finish the lab quickly, but again, do not rush. Take your time and try out new things. Get job ready!
