# Hunting Metasploit

In this following lab, we will be focusing on hunting artifacts related to metaspolit with the help of sysmon,  powershell and FilterXPath

The following commnd can be used to filter through entries in the suspicious.evtx file

`Get-WinEvent -Path C:\Users\THM-Analyst\Desktop\Scenarios\Practice\suspicious_file.evtx -FilterXPath '*/System/EventID=3 and */EventData/Data[@Name="DestinationPort"] and */EventData/Data="4444"'`


<add screenshot>
