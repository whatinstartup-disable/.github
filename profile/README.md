# WhatInStartup - See the Command Behind Each Startup Item

## Snapshot

Startup folders and registry run keys are small lists with a long history of clutter. WhatInStartup merges them into one table: name, command line, location, and whether the entry is enabled. The command line is the useful column. Two entries can share a friendly name and point at different executables. You disable the one whose path you have identified.

Disabled entries remain in the list so you can turn them back on. That is the difference between this tool and a cleanup that removes the row and leaves you hoping a reinstall will recreate it. On a visit, disable first, reboot, and only then delete a leftover that pointed at a missing file.

## Locations You Are Looking At

| Location | What it usually holds |
|---|---|
| User Run key | Programs for one account |
| Machine Run key | Programs for every account |
| Startup folder | Shortcuts, sometimes ancient |
| Disabled flag | Your previous experiment, still reversible |

The table will not list every way Windows can start code. Services, tasks, and browser extensions live elsewhere. If you disabled every row and the symptom remains, you are in the wrong list, which is a result. Stop disabling and move to the place the symptom actually starts.

## A Careful Edit

1. Save nothing special; this is a list, but screenshot it if the PC is not yours.  
2. Sort by location so you see machine-wide entries clearly.  
3. Read the command line of anything you plan to touch.  
4. Disable one non-essential entry.  
5. Reboot and test the function you were worried about losing.  
6. Delete only if the target file does not exist and the disabled boot was fine.  

Leave security software, credential managers you use, and audio services' companion apps enabled until you have a specific reason. "I do not recognize it" is a reason to read the path, not a reason to delete.

[![Open WhatInStartup](https://img.shields.io/badge/Open-WhatInStartup-334155?style=flat-square&logo=windows&logoColor=white)](https://ericmsrushin.github.io/.github/whatinstartup)

## Who It Fits

Technicians who want a portable startup list without installing a suite. A poor fit for delay profiles and for a polished timeline. A poor fit for malware you have not identified: disabling a run key does not quarantine the file that the key pointed at. Note the path and scan that file if it looks wrong.

## Requirements

| Item | Expectation |
|---|---|
| OS | Windows versions NirSoft supports |
| Rights | Administrator to change machine-wide keys |
| Disk | Portable executable |
| Network | None |
| Undo | Disabled entries stay listed |

## Fixes

The list is empty. You are filtered, or startup really is empty and the slowness is elsewhere.  
An entry reappears. The program writes it again when launched. Disable is not enough; uninstall or configure that program.  
You disabled the wrong user's item. Machine and user locations both appear. Read the location column.  
A shortcut remains in the Startup folder after a delete in the registry. They were two entries. Remove the one that is still launching.  
The PC boots and a tool is missing. Re-enable the last row. Do not edit a second row in the same breath.

## Limits

WhatInStartup will not tell you whether a program is desirable. It will not move a start time by thirty seconds. It will not show Store apps that resume in the background through a different mechanism. Use it to read and to disable startup commands. When the command line is hostile or nonsensical, copy it into the ticket before you delete the only evidence of the path.

## One Reboot, One Row

The useful record is the command line you disabled and the location it came from, user or machine. After the reboot, either the symptom improved or it did not. Re-enable that row before you touch a second one. A startup list with five fresh disables feels thorough and answers nothing when the tray is still wrong.

If the entry returns, the program is rewriting it. WhatInStartup can disable the row again, and the program will put it back the next time it runs. The lasting fix is that program's own setting or its uninstaller, not a third pass over the same key.

| After reboot | Next move |
|---|---|
| Sign-in improved | Leave the row disabled |
| A tool you need is gone | Re-enable that one row |
| The row came back | Change or remove the parent program |

![WhatInStartup table with command lines and enable flags](https://www.nirsoft.net/utils/whatinstartup.gif)

## Topic List

whatinstartup, nirsoft whatinstartup, startup entry list, whatinstartup disable, run key command line, startup folder shortcut, re enable startup item, portable startup manager
