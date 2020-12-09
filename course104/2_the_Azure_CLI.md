# The Azure CLI

These labs are about the Azure CLI. This is a command line tool. If you pick Linux, Microsoft learn shows you the command for a Debian / Ubuntu based Linux. If you use a different type, you have to google. 
I use OpenSuse therefore I have to install it with: https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-zypper

The az login command will open a browser window. If you have multipe browsers, you can copy the link approval link to a diffrent browser.

## recommendations
- This is a 4 hour lab, you have a lot of time to play around.
- Do not rush, you can finish the lab in 10 minutes, but your goal is knowledge!
- You can use this lab to get the big picture and you can do a lot of bonus things for free.


## Why is this lab important?

As an admin, command line tools are often faster and the Azure sandboxed labs have problems with the shell. If you use your machine, you always get access to the Azure CLI.


https://docs.microsoft.com/en-us/learn/modules/control-azure-services-with-cli/3-exercise-install-and-run-the-azure-cli/

https://docs.microsoft.com/en-us/learn/modules/control-azure-services-with-cli/5-exercise-create-website-using-the-cli/

Tasks:
- You create a service plan. Describe what a service plan is. What is --sku FREE?
- Open Azure Portal (https://portal.azure.com/) and log in. Describe in detail what you did via command line and where you can find these things via the portal.

You can look for the app service plan and the app service:
- What it the matching value for --sku FREE? Your sandbox runs 4 hours, but how long can you have your web running per day?
- Are these things IaaS, PaaS or SaaS?

Bonus tasks:
- The resouce group allows you to use and activate Application Insights for your resources. Activate it. Discover the feature. Why is this feature very useful?
- Try to create a working alert rule with the following setting: Scope: your webapp, Condition: CPU higher 1%, Action: send an email to your account every 5 minutes. Specify a name, create a alert rule. -> this will not work, a policy disallows it, but you can do the steps.
