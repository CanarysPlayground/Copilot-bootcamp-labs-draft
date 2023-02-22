# Objective

Create a nodejs script to get all repositories and their respective sizes from an organization using GitHub CoPilot

## Note

- CoPilot is there to help you code and give suggestions. 
- Any user using Copilot must have some or more knowledge on the platform and the scripting language in which they are writing code
- Any suggestions given by CoPilot must be reviewed and modified according to specific requirement.

## Pre-requisites

- NodeJS is installed on the developers machine
- GitHub user account
- CoPilot License for the user is activated 
- VSCode is installed on the developers machine
- GitHub CoPilot extension for VSCode is installed

### CoPilot Lab

- Open your Visual Studio Code Instance
- From the terminal create a new folder, open the folder in VScode workspace
- Create a new file githubrepos.js
- Add a brief comment 

![image](https://user-images.githubusercontent.com/67369513/220420397-fbf161be-4ffc-472a-b522-23a47addbe51.png)

- CoPilot will give suggestions on the libraries to use for running your script. Choose an appropriate one or add your own inputs

![image](https://user-images.githubusercontent.com/67369513/220421202-2f631ae8-7a6a-425b-9422-722ac04f8238.png)

- Add variables to accept github organization name and github token as inputs to authenticate with the GitHub API
- Add a comment to get the repository size. Add a function name, copilot will suggestions on the required code to get the repository size information. CHoose the appropriate one

![image](https://user-images.githubusercontent.com/67369513/220424608-09072c53-10c5-45fd-9d08-c4ab9713b10d.png)

- Add a new comment to create the csv file, copilot will populate a suggestion. Choose the required one and make changes if necessary
![image](https://user-images.githubusercontent.com/67369513/220425309-ee284d39-69fe-4fd7-84be-525bbfa563fb.png)

- Copilot will automatically suggest to add lines for writing the repository data to csv file. 
![image](https://user-images.githubusercontent.com/67369513/220426043-c4c41371-e403-438a-bd42-64758412593c.png)
![image](https://user-images.githubusercontent.com/67369513/220426227-a562fee7-2ac0-4402-9134-80777b416bf6.png)
![image](https://user-images.githubusercontent.com/67369513/220510839-8528bc80-529a-4a4b-8b30-99c90e3a7bf3.png)

- Add a package.json or run npm init and install the required modules by running npm install
![image](https://user-images.githubusercontent.com/67369513/220511267-e2a4c262-3a54-4250-ad2f-dc46d36cce27.png)

- Run the script by running command node githubrepos.js. Check the generated csv file
![image](https://user-images.githubusercontent.com/67369513/220512804-7a4d7812-c546-4d83-8840-3f174c214640.png)



