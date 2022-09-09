# Aggressor-CS 4.0+

My developed set of Aggressor Scripts for Cobalt Strike 4.0+



- **`remove-beacon.cna`** - This script gives the operator the ability to **kill** a beacon session through the command-line instead of clicking through the Beacon Session Table manually.

```
beacon> help bye

Description : 

Exit Session and Remove from Display

```


- **`save-output.cna`** - This script helps the operator to save long output of commands ran in the command-line. For example, the output of a program might reach the output limit of the beacon terminal or causes inconvenience to scroll to the very top to copy paste the output to a file. By using this module, the output of the command is automatically saved into the filename specified.

```
beacon> help saveoutput

Supported Modules : (execute-assembly,run,shell,powerpick,powershell)

Usage : saveoutput filename module command optional_arguments

Examples : 

saveoutput seatbelt_output.txt execute-assembly /opt/Seatbelt.exe "-group=system"
saveoutput netstat.log run net "localgroup Administrators"
saveoutput process_list.txt shell whoami "/all"
saveoutput usernames.txt powerpick Get-DomainUser
saveoutput jaws.txt powershell C:\Tools\JAWS.ps1
```
<br>

  - **Important Note (save-output.cna) :** Operator is required to reload save-output.cna script before execution to avoid output repetition bug to occur.

<br>

![script](https://raw.githubusercontent.com/mohinparamasivam/Aggressor-CS4.0/master/images/script.png)


