## These are the sand boxed AZ-104 labs

- you do not need an Azure account.
- You need a Microsoft accout, that is it
- If you want, you can create an Azure account, there are two options. The free one and a student version (you need an *edu mail).
- The most labs are sand boxed, you cannot do anything wrong.
- The most labs are 1 hour

Hint:
- you cannot pass the exam with doing the labs alone, but I like hands-on.
- In my opinion, it is easier to understand the theoretical part, after you saw the topic in a real scenario
- If you want to learn effectively, do more! Try to understand the labs a click around. Some labs have hidden "premium" features activated. -> Always check the learn resource group and click on all unknown items. 

### Let us dive in

https://docs.microsoft.com/en-us/learn/modules/intro-to-azure-virtual-machines/3-create-a-vm/

Here you create a VM. If you have a free Azure account, you can create a VM for free, but this lab offers you a Standard D2s V3 tier. This is more powerful than your free machine, but you only have 1 hour to play around.

Bonus tasks:
- Do the lab, but if the guide motivates you to do something, do not skip it. This lab is free and you can do a lot. You can install a Ubuntu 20.4. 
- Think about inbound port rules. What is a port? 
- Discover the Disks section. Can you find details about Premium SSD vs Standard HDD?
- Connect to your VM with ssh. Open a shell on your computer and use ssh to connect> ssh stefan@23.101.203.57 (example for linux). If you use Windows, you need to download Putty first or use the Windows 10 tool (https://www.howtogeek.com/311287/how-to-connect-to-an-ssh-server-from-windows-macos-or-linux/)
. 

### Advanced task (you need to google)
Example to install a GUI on your Linux system (https://docs.microsoft.com/en-us/azure/virtual-machines/linux/use-remote-desktop)

Login via ssh
ssh azureuser@myvm.westus.cloudapp.azure.com or ssh stefan@23.101.203.57

Install all tools

The commands

sudo apt-get update  -> updates the system, takes a while

sudo apt-get -y install xfce4   -> installs the GUI

sudo apt-get -y install xrdp  -> installs remote desktop

sudo systemctl enable xrdp

echo xfce4-session >~/.xsession

sudo service xrdp restart

Now, you try to connect to the Linux, but it will not work. Why?

RDP needs port 3389 open, but we allow only port 22.
Find the network tap (test-ubunto-nsg) and add 3389.

Find a way to connect. If you have windows, it is very simpe. In your Azure portal find the virtual machine and the connect button. Download the rdp file and click on it. -> you are in.
