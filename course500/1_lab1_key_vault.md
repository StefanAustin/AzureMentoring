## Key vault labs

- https://docs.microsoft.com/en-us/learn/modules/manage-secrets-with-azure-key-vault/3-creating-vaults-storing-secrets/
- https://docs.microsoft.com/en-us/learn/modules/manage-secrets-with-azure-key-vault/5-access-secrets-from-web-app/
- https://docs.microsoft.com/en-us/learn/modules/manage-secrets-with-azure-key-vault/6-configure-deploy-run-azure/

### Hint:
Sometimes, the Azure Cloud Shell is black and you cannot do anything. Solutions:
- Refresh the browser
- Use the Azure portal to connect. Next to the seach bar is a Cloud shell button. Click on it.
- if it does not work, sign out and sign in again.
- if it does not work switch to the powershell option and back
- if it does not work restart the shell
- if it does not work go back to the lab web page, sometimes you can restart the shell

--> it is a Microsoft product and not reliable. Azure feels like Win95. Sometimes I need 7 minutes to get a shell :( The first lab is a 4hour lab, so it does not really matter.

## Lab 1

Questions:
- What is a key vault and what can you store?
- Log in via Azure Portal and see what you did. Find the key vault and inspect Keys, Secrets and Certificates. Can you create another secret via the portal?
- What is the diffrence between a key and a secret? Let us say you have a disk and you want to encryt the disk, what should you use? Secret, Key or Certificate?
- Try to create a Key.

Save the key vault name.

### Bonus part:
The next section is about managed identities.  -> This is exam relevant
- Describe managed identity in a sentence. 
- Why do you need it? 
- Do you need a Premium P2 licence for it? 
- How does it work? Maybe draw a simple picture.
- What is a token?

## Lab 2

This lab opens an editor. It will take a while (~10 minutes for the second step).

The save button is very hidden. Look for the the dots.
Command: touch Controllers/SecretTestController.cs has to go into the Azure shell, not in the editor. Refresh the editior.
- Insert the code and SAVE it.

## Lab 3
Insert your app service plan name, most likely it is: keyvault-exercise-plan

The lab does not really work. Try to use the Azure portal to see what you did.
