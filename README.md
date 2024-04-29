# Common Helpdesk functions using Active Directory
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>

### Objective<h2>

This Active Directory Lab project aimed to farther my understanding of Active Directory functions to gain preparedness in real-world helpdesk scenarios. The primary focus was to ingest and stregthen my knowledge within the Mircosoft Server application system, generating test telemetry to mimic real-world helpdesk tasks.

### Skills Learned<h2>

- Understanding of Active Directory concepts and practical application.
- Proficiency in creating new accounts in Active Directory.
- Ability to generate and recognize common Active Directory features.
- Development of critical thinking and problem-solving skills in Helpdesk.

### Tools and Technology Used<h2>

  - Microsoft Azure (Virtual Machines/Computers)
  - Remote Desktop
  - Active Directory Domain Services
  - Windows Server 2022

## Steps

* **Adding a new user account using the "Copy" method.** <p>
The one feature that can containurized and mantain users, computers, and OUs is the task "Active Directory "Users ans Computers." This method allows you to automate adding new user accounts by replicating account permissions.
  - Click on the tools tab and under the drop box click "Users and Computers"
  - Click the "Users" folder
  - Find the user you want give the same permissions too. Right click and hit "copy." In the photo below we created a new admin account user named "Jason Tatum" with all the same permissions as a Domain User.
![AD users computers](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/21d536a2-552d-4d7e-b42c-b068b0f29961)
![copy 2](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/55cfbba5-f666-4688-a90a-93de45da4983)


* **Finding a user profile**<p>
In order to find a user, contact, or group in Active Directory you make sure and search "Entire Directory." This important because the user you are searching could be aprt of a different folder or OU.
  - Right click the "Computers" envelope. Click "Find"
  - Type in the user's name and click "Entire Directory" under the drop box in the photo shown below. Finally click "Find" to search entire directory.
![fins user](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/2b7ae503-ba3d-4896-a326-6f1c669e3cd8)
![entire direcroy](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/680d8202-59ec-415b-91b8-c5ba3520fe60)<p>

* **Enable Recycle Bin**<p>
  - Click Windows Adminstrator
  - Click Active Directory Adminstrator Center.
  - Click your Domain Server.
  - Click "Enable Recycle Bin" on the right side of the computer screen and press "ok."
  - This enables a "Delected Objects" folder to use and regain objects.
  ![recycle bin ](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/49d38e4f-34d3-4e75-b58d-a83701d6ec58)
  ![bin 2](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/95f03229-3d6d-46c2-af5f-227ce3cb8f22)
  ![bin 3](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/a6c7a693-1479-4b0d-a846-b9aee70882ba)

* **Cmd Command for password expiration**<p>
The "net user" command deatils when the account's password expires
  - Open Cmd command line . Type "net user (user name) {space} /domain."
![AD cmd](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/15378c80-a98d-4106-9b9f-338bafb31b55)

* **Unlock a user account in Active Directory**<p>
A common helpdesk issue is someone being locked out of their account. Below is the documentation to fix the user's issue.
  - Open Server Manager.
  - Search the user. Double click the user.
  - Click the "account" tab.
  - Check the "Unlock account" box and press "Ok."
 ![unlock account](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/79ebd364-6409-4bb1-8e09-5b7468aeb139)

* **Reset the Users passwords in Active Directory**<p>
If user has forgotten their password and can no longer access desktop you can go into Domain Controller, reset passsord and give them a new password.
  - Open Server Manager.
    Search the user. RIght click the user's name.
  - Click the "Reset Password."
  - Enter new password and press "Ok." Provide feedback to user with new password.
![reset2](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/86b7a913-93a9-42f6-a4c3-c9b7c383f100)
![pass reset](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/0f930cbd-b43d-4143-9720-5b3233440683)

* **Create a shared drive permissions for security groups**<p>
  (4/21/24) Lab 7 {Bookmark}
  
* **Printer Set up for Server Manager**<p>
- Click "Add Roles and Features" then click "next" until the "Select server roles" menu appears
- Click "Print and Document Services" click "next" until the "Install" appears and start installion progress.
- Click "Tools" and select "Print Management"
- Right click "Add printer" then select "Add a new printer using existin port"
- Click "Install a new driver"
- Select printer in this case I selected " " then click until finished.
- The last photo you right click the printer and press "Properties" then select the "Security" tab. This feature allows you add/remove users for the printer and shows who has printer persmissions. 
![printer](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/bfc23d06-fe64-40e4-b77c-687e2920623d)
![printer2](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/316a35b0-847a-485a-88f4-2eecb383ce37)
![print3](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/6d4c293f-7ad5-4684-a525-660671945ceb)
![print4](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/fa711a73-a910-4bcf-9ab0-b59dd191f7dc)
![print6](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/6cadacc1-9d23-4628-a0fa-873fe0da3e58)
![print7](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/dd4cf037-9499-49f8-916d-da8875a2b585)
![printer7](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/7aa88453-39eb-4bfe-82df-37e8b16f4e6b)
![printer8](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/2bc9f9c1-7337-487c-8dd4-e22b23df5afe)
![printer9](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/04415085-81e8-462d-b802-522e96f38f97)
![printer10](https://github.com/TerrellSowell/Helpdesk-functions-Active-Directory-account-creation-Cmd-Commands-/assets/161978506/7e291ae4-fb84-4feb-bec0-a52669cc43c6)


   


  



