## [EMS] Epoch Mission System 
### Version 0.3.1
#### Based on Vampire's DZMS 1.1 Final Edit
##### Updated and revamped slightly by Defent July 12, 2014.
> http://opendayz.net/threads/beta-dzms-dayz-mission-system.18421/ 
> http://epochmod.com/forum/index.php?/forum/49-epoch-mission-system/

(Let their bodies hit the floor)

**Requirements**:

   Notepad++ 
	http://notepad-plus-plus.org/
   Notepad++ sqf addon 
	http://www.armaholic.com/page.php?id=8680
   PBO Manager
	http://www.armaholic.com/page.php?id=16369
   Epoch 1.0.4+ Server

**Difficulty** :

    Some knowledge of Epoch Server & Mission file locations
    How to use PBO manager to unpack and pack PBO files
    Easy : ~ 5 minutes

--------------------------
Installation
--------------------------
1.	Download the Github Zip folder and open it with your unPacker of choice. You can also download
	Defent's forked version in the 2nd link below.

	> https://github.com/TheFuchs/EMS-0.3/archive/master.zip
	Defent Edit
	> https://github.com/Defent/EMS-0.3
	
2.	Extract it to your Desktop or somewhere where you won't lose it.
	Inside the Zip is this Readme.MD, a folder called Documentation, and one called EMS.
	
3.	Open your Server.PBO with the PBO unPacker of your choice.

4.	Put the "EMS" folder into your Server.pbo.

5.	Open up your server_monitor.SQF in the system folder in your server.PBO.

	Search for this line
	
	```allowConnection = true;```
	
	And insert this line directly above it.<br />
	```[] ExecVM "\z\addons\dayz_server\EMS\DZMSInit.sqf";```
	
	If you have DZAI or WickedAI Installed, the DZMS line should go under theirs.
	
6.	(Optional) Change the settings in DZMSConfig.SQF.

7.	(Optionally Optional) Adjust the files in the ExtConfig folder.
	
8.	Now just rePack your PBO and enjoy!
