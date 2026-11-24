This program reads the LIVE player avatar stats from the game client's memory and displays it in a format different from the game.  Use it to make gear swap decisions or see the effects of various buffs and debuffs in real-time.

Compiling this requires AutoIt v3.  It must be compiled as a 64-bit application for 64-bit systems.  Windows is the only supported OS and there are no plans to port this to Linux.

Elevated privileges (admin) may be required to read the game's memory, depending on your system configuration.  This program does not read or write to or from any drive after loading, nor does it have any network connectivity capability.  It does not inject any code into the game or modify any values it reads.

Some virus scanners may report AutoIt compiled programs as malicious.  A virus scan result can be found here:
https://www.virustotal.com/gui/file/56837351c00b5202a3e02472fb6c1bc581edcb075bd229cc62f893ade4b7efa3


How to use this program:
It is a portable exe and can be placed in any directory.
Run it alongside the game.  It does not matter which is launched first.

The - and + buttons in the top-left resize the application.

The program will detect any changes to your hero's stats in real-time.  If you want to compare gear, it is strongly recommended to stay in a controlled area (like the training room) to avoid player auras from causing a stat update.  Some heroes and items have buffs that apply themselves when moving or after stopping, so keep that in mind.
Checking the "Lock Old" box will read your stats immediately so you can compare against a baseline.  Checking the other boxes will not cause the program to read your stats, but it will change the calculations to match OFFENSE only for powers tagged with those boxes, and brutal immune for CoA server.


How this calculates and displays information, different from in-game:
Defense includes an average of your physical, mental, and energy defenses added to your defense rating because we don't know what type of damage you will be receiving.  In general, very few items add to these stats.  If you have those items equipped, expect your defense in the program to be higher than the game shows.

Mitigation in the program includes all sources of mitigation:  damage reduction from gear, defense, deflect, and dodge.  Mitigation can exceed 90% because of dodge and deflect reducing hits.  Mitigation displayed will likely be higher than the "damage reduction" stat shown on your character sheet.

Crit chance shows your REAL crit chance.  Brutal chance is the chance to CONVERT your crit to a brutal, so if you increase your brutal chance without changing your crit chance, your REAL crit chance goes down.  This is a good thing.

The number displayed to the right of Offense in the New column is a comparison of final DPS from old to new.  It uses a theoretical power with 1 damage as the baseline and shows how much that power would change.


What this program doesn't do:
Programming to account for every hero and every situation would be a mountain of a task.  Some powers don't benefit from attack speed, and some do.  Some heroes benefit from increases to max spirit.  Some benefit from max health, but only on certain powers.  Those changes are not accounted for.  
For most situations, however, this program can give you a very good idea of how much DPS and survivability is changed by glancing at the Offense change and mitigation/EHP change.
