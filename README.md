# Megamek Startup Scripts (1.2.0)
Startup scripts for the MegaMek game server software - uses the "screen" command to manage the session. This also restarts the Megamek server process if it crashes.

Official support sites: [Official Github Repo](https://github.com/fstltna/MegamekStartup) - [Official Forum](https://mekcity.gameplayer.club/index.php/forum/our-utilities)

---

These start up the MegaMek server at boot time with a "screen" process.

1. Copy **megamek** into **/home/mekuser/bin** - make sure it is executable
2. Copy **startmegamek** into **/home/mekuser/mekhq** - make sure it is executable
3. Copy **MegaMekProcess** into **/home/mekuser/mekhq** - make sure it is executable

When you want to view the Megamek console, just enter "**screen -r**" in your shell.

To disconnect from the Megamek console just press **CTRL-A CTRL-D**. This will leave it running and you can reconnect to it again.

I have only tested this on a Ubuntu 24.04 server...

If you want to turn off the server respawning type "**touch /home/mekuser/mekhq/nostart**". To reenable it type "**rm /home/mekuser/mekhq/nostart**".

---
Note: If you don't already have the "screen" tool installed you will need to install it by "**sudo apt-get install screen**".
