# Virtual Garage for Exile
###### Made by Shix
Virtual garage is just what it says its a virtual garage system for Exile

---

### Installation
---
### Server Side
1. Open your mySQL database editor
2. Copy and paste the contents of **VirtualGarage.sql** in to the query
3. Run the query
4. Refresh your database and you should now have one new table
  * virtual_garage
5. you are now done with database changes so you can close your mySQL editor
6. Navigate to **@ExileServer/extDB/sql_custom_v2**
7. Open up the **exile.ini**
8. Copy and paste the contents of **VirtualGarage_extDB2.ini** at the bottom of exile.ini
9. Save **exile.ini**
10. Copy the **VirtualGarage_Server.pbo** into **@ExileServer/addons**
11. De-PBO your **exile_server.pbo**
12. Copy the **ExileServer_system_network_dispatchIncomingMessage.sqf** from the Exile Overwrites and paste it in to your exile_server/code folder
13. Re-PBO your **exile_server** folder

### Client Side
1. De-PBO your mission File
2. copy the **VirtualGarage** in to the root of your mission file
3. open up your config.cpp
4. Locate `class CfgInteractionMenus`
5. within CfgInteractionMenus find the `class Laptop`
6. Copy and paste the class VirtualGarage from config.cpp file you downloaded from github in to the Class Actions
7. Scroll all the way to the bottom of config.cpp copy the CfgNetworkMessages & VirtualGarageSettings and paste it at the bottom of config.cpp
8. Save your config.cpp
9. Open your description.ext scroll all the way to the bottom, Open up description.ext from the files you downloaded from github and paste the contents at the bottom of your description.ext in your mission file
10. Open up your init.sqf
11. paste `execVM "VirtualGarage\VirtualGarage_Client_Init.sqf";` inside
12. Save your init.sqf
13. Re-PBO your mission file
14. That's it your done

---
### Additional Info
you can configure the virtual garage setting via VirtualGarageSettings that you placed at the bottom of your config.cpp in your mission file

This script was only written in about 2 days so may not be perfect so if you do find any bugs please post them on the forum post or message me on the Exile mod Forum

If you have anything you would like to see added also feel free to post on the Forum post with your suggestion
