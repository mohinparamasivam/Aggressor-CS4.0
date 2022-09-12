# Aggressor-CS 4.0+

My developed set of Aggressor Scripts for Cobalt Strike 4.0+



- **`remove-beacon.cna`** - This script gives the operator the ability to **kill** a beacon session through the command-line instead of clicking through the Beacon Session Table manually.

```
beacon> help bye

Description : 

Kill Beacon and Remove from Display

```

**Example :** Notification is sent when user kills beacon<br><br>
![Kill Beacon](https://raw.githubusercontent.com/mohinparamasivam/Aggressor-CS4.0/master/images/kill_beacon.png)<br><br>



https://user-images.githubusercontent.com/28557040/189568936-a3505727-e6a8-443b-9209-d284dc7e7e7d.mp4



- **`save-output.cna`** - This script helps the operator to save long output of commands ran in the command-line. For example, the output of a program might reach the output limit of the beacon terminal or causes inconvenience to scroll to the very top to copy paste the output to a file. By using this module, the output of the command is automatically saved into the filename specified.




```

beacon> help saveoutput

Supported Modules : (execute-assembly,run,shell,powerpick,powershell)

Usage : saveoutput filename module command optional_arguments

Examples : 

saveoutput seatbelt_output.txt execute-assembly /opt/Seatbelt.exe "-group=system"
saveoutput netlocalgroup.log run net "localgroup Administrators"
saveoutput whoami_full.txt shell whoami "/all"
saveoutput usernames.txt powerpick Get-DomainUser
saveoutput jaws.txt powershell C:\Tools\JAWS.ps1
```
#### Example : 
![Example Usage](https://raw.githubusercontent.com/mohinparamasivam/Aggressor-CS4.0/master/images/example_saveoutput.png)
<br><br>

  - **Important Note (save-output.cna) :** Operator is required to reload save-output.cna script before execution to avoid output repetition bug to occur.

<br>

![script](https://raw.githubusercontent.com/mohinparamasivam/Aggressor-CS4.0/master/images/script.png)


https://user-images.githubusercontent.com/28557040/189569256-8834d4e7-964d-4786-b5bd-a1bafffe4860.mp4





