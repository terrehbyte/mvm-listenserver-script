TF2 MvM - Listen Server Script
==============================

Brief
-----

This script simplifies the process of setting up and running an MvM listen server. It allows the server to run a config to prep the server for MvM, select an MvM map, and then change the difficulty at any given time during the game.

It is intended for use amongst friends for those who do not want to install Metamod and Sourcemod but still want to be able to adminstrate and manage a listen server.

Installation
------------

0.  This assumes that your client is already capable of hosting TF2 servers.

1.  Navigate to your Team Fortress 2 installation location. That would be:

    /Steam/steamapps/common/Team Fortress 2/

2.  Next, make a folder in your custom content folder.

    /Steam/steamapps/common/Team Fortress 2/tf/custom/<NEW_FOLDER_NAME>/

3.  Create a "cfg" folder in the newly created folder.

    /Steam/steamapps/common/Team Fortress 2/tf/custom/<NEW_FOLDER_NAME>/cfg/

4.  Download the configs in this repo and place them in your newly created "cfg" folder.

    /Steam/steamapps/common/Team Fortress 2/tf/custom/<NEW_FOLDER_NAME>/cfg/mvm_master.cfg

    /Steam/steamapps/common/Team Fortress 2/tf/custom/<NEW_FOLDER_NAME>/cfg/mvm_decoy.cfg

    ...and so on and so forth.

5. Edit mvm_master.cfg, changing the hostname and password to your liking.

Usage
-----

1.  Launch Team Fortress 2 and open up the console.

2.  Run the command

	exec mvm_master.cfg
	
    This preps your client for hosting an MvM listen server, setting needed variables.

3.  Type in the name of your desired map. (i.e. BigRock, Decoy, etc.)

4.  Upon map load, the console should contain a list of commands and the difficulties that correspond with them. Enter the corresponding command to change the difficulty.

    For example, if you are on the map "mvm_decoy," you can type, "Decoy1," without the quotation marks to load the first difficulty, "Doe's Drill." Those commands can be run at any time and can be used to reload the game without actually reloading the map.