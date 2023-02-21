# Creating Copilot with your Codespace

In this hands-on lab you will use Codespaces and Copilot to utilize the benefits that Copilot gives to developers writing code. Good luck! 👍

This hands on lab consists of the following steps:

- [Creating first codespace](#creating-first-codespace)
- [Add devcontainer and devcontainer json file](#add-devcontainer-and-devcontainer-json-file)
- [Code with Copilot](#code-with-copilot)
- [If time permits add additional methods](#if-time-permits-add-additional-methods)

## Creating first codespace

1.	Work inside your current repository `<org-name>/<repo-name>`
2.	Under the repository name, use the Code drop-down menu, and in the Codespaces tab, click Create codespace on main.

      ![image](https://user-images.githubusercontent.com/95218310/220299736-f35a5584-2e92-4628-bbe1-120f3f61c359.png)

3.	Wait for the codespace to spin itself up. Note, it’s a VM spinning up in the background.
4.	Once your codespace is created, your repository will be automatically cloned into it.

## Add devcontainer and devcontainer json file

1.	Inside your codespaces Add a `.devcontainer` folder and `devcontainer.json` in the root of your Repo
2.	Click "Add File"
3.	Click "Create New File"
4.	Type or copy paste.

```
.devcontainer/devcontainer.json
```
5.	In the body Add the following customizations.

```
	{
	  "name": "Codespace to bootstrap GitHub Action Importer in a Codespace",
	  //Use base codespace image then pull GitHub Action Importer on postCreateCommand,  
	  "image": "mcr.microsoft.com/vscode/devcontainers/universal:linux",
	  "remoteEnv": {
	    "DOCKER_ARGS": "--network=host",
	    "INSTALLATION_TYPE": "labs"
	  }
	  ,    
	  // Add the IDs of extensions you want installed when the container is created.
	  "customizations": {
	      "vscode": {
	          "extensions": [
	              "GitHub.copilot"
	          ]
	      },
	      
	  }
	}
    
 ```
 
 6.	Save the changes, then on the right corner you will see the notification to Rebuild the container. Just click on the Rebuild Now.

     ![image](https://user-images.githubusercontent.com/95218310/220301410-f2b13df5-deba-44fe-9767-b22b733077f6.png)

7.	Wait for the codespace to spin itself up. Note, it’s a VM spinning up in the background.
8.	Then The copilot extension should show up in the VS code extension list.
9.	On the bottom right of the screen there should be a Copilot icon. Hover over the icon.
10.	Verify the text says Deactivate Copilot as below

      ![image](https://user-images.githubusercontent.com/95218310/220301812-76993025-addc-4d53-af6b-f5a21b39be4d.png)

## Code with Copilot

1. Add a new files in VSCode called `Bootcamp.cs`
2. Inside the new file type `public class Bootcamp`
3. CoPilot will suggest code to finish creating the class.

    ![image](https://user-images.githubusercontent.com/95218310/220301997-ccdddc83-3425-4327-9692-bf6b1fc73a29.png)  

4. Accept the code suggestion.

## If time permits add additional methods

1. Get creative and see what you can do to have Copilot suggest code.
