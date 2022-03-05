# Implementation 
## Research
### Splunk
+ [Splunk MITRE App](https://splunkbase.splunk.com/app/4617/)
+ [Find the contetnt that masters most](https://www.splunk.com/en_us/blog/security/splunk-security-essentials-3-1-with-enhanced-mitre-att-ck-matrix-find-the-content-that-masters-most-to-you-faster.html)
+ [detecting cyber threats with MITRE ATT&CK app for splunk : part 1](https://medium.com/seynur/detecting-cyber-threats-with-mitre-att-ck-app-for-splunk-a6627439a9e3)
+ [detecting cyber threats with MITRE ATT&CK app for splunk : part 2](https://medium.com/seynur/detecting-cyber-threats-with-mitre-att-ck-app-for-splunk-part-2-c07c68ce1b03)
+ [DA-ESS-MitreContent](https://github.com/seynur/DA-ESS-MitreContent)
+ [DA-ESS-MitreContent](https://seynur.github.io/DA-ESS-MitreContent/versions/1x/)
+ [youtube](https://www.youtube.com/watch?v=Y6jiFsa7vT0)

### Logstash and ElasticSearch
+ [How to use mitre attack](https://www.elastic.co/pdf/how-to-use-mitre-attack)
+ [Visualizing MITRE round 2 evaluation results Kibana](https://www.elastic.co/blog/visualizing-mitre-round-2-evaluation-results-Kibana)
+ [signals in elastic siem sysmon data](https://www.elastic.co/blog/signals-in-elastic-siem-sysmon-data)
+ [MITRE engenuity attck round 3 carbanak fin7 vs free open elastic security](https://www.elastic.co/blog/mitre-engenuity-attck-round-3-carbanak-fin7-vs-free-open-elastic-security)
+ [elsec_dr2an](https://github.com/ElasticSA/elsec_dr2an)
+ [Security assessment using elastic security siem](https://medium.com/security-assessment-using-elastic-security-siem/introduction-db745c172cf9)




## splunk mitre searches
### Techniques

|number|Rule Name|MITRE Techqniue|
|:-|:--------|:--------|
|1 |Execution with AT|[T1053.002](https://attack.mitre.org/techniques/T1053/002/)|
|2 |Running executables with same hash and different names|[T1036.003](https://attack.mitre.org/techniques/T1036/003/)|
|3 |Active Directory Dumping via NTDSUtil|[T1003.003](https://attack.mitre.org/techniques/T1003/003/)|
|4 |Squiblydoo|[T1218.010](https://attack.mitre.org/techniques/T1218/010/)|
|5 |Services launching Cmd|[T1543](https://attack.mitre.org/techniques/T1543/)|
|6 |Credential Dumping via Windows Task Manager|[T1003.001](https://attack.mitre.org/techniques/T1003/001/)|
|7 |UAC Bypass|[T1548.002](https://attack.mitre.org/techniques/T1548/002/)|
|8 |Command Launched from WinLogon|[T1546.008](https://attack.mitre.org/techniques/T1546/008/)|
|9 |Host Discovery Commands|T1087 T1069 T1016 T1082 T1033 T1057 T1007|
|10|Create Remote Process via WMIC|[T1047](https://attack.mitre.org/techniques/T1047/)|
|11|Generic Regsvr32: Main Pattern|[T1218.010](https://attack.mitre.org/techniques/T1218/010/)|
|12|Generic Regsvr32: Spawning Child Processes|[T1218.010](https://attack.mitre.org/techniques/T1218/010/)|
|13|Powershell Execution|[T1059.001](https://attack.mitre.org/techniques/T1059/001/)|
|14|Suspicious Arguments|T1003 T1021 T1105|
|15|Lsass Process Dump via Procdump: Process Create|[T1003.001](https://attack.mitre.org/techniques/T1003/001/)|
|16|User Activity from Clearing Event Logs (Security)|[T1070.001](https://attack.mitre.org/techniques/T1070/001/)|
|17|Simultaneous Logins on a Host|[T1078](https://attack.mitre.org/techniques/T1078/)|
|18|Execution with schtasks|[T1053.005](https://attack.mitre.org/techniques/T1053/005/)|
|19|Quick execution of a series of suspicious commands|T1087 T1003 T1069 T1057 T1021 T1543 T1112 T1574 T1018 T1569 T1053 T1029 T1033 T1007 T1082 T1049 T1016 T1010 T1518 T1046 T1562 T1098 T1059 T1012|
|20|Reg.exe called from Command Shell|T1012 T1112 [T1547.001](https://attack.mitre.org/techniques/T1547/001/) T1574|
|21|Remote PowerShell Sessions|[T1059.001](https://attack.mitre.org/techniques/T1059/001/) T1021|
|22|User Logged in to Multiple Hosts|[T1078](https://attack.mitre.org/techniques/T1078/)|
|23|Suspicious Run Locations|[T1036.005](https://attack.mitre.org/techniques/T1036/005/)|
|24|Processes Spawning cmd.exe|[T1059.003](https://attack.mitre.org/techniques/T1059/003/)|
|25|RDP Connection Detection|[T1021.001](https://attack.mitre.org/techniques/T1021/001/)|
|26|RunDLL32.exe monitoring|[T1218.011](https://attack.mitre.org/techniques/T1218/011/)|
|27|Successful Local Account Login|[T1550.002](https://attack.mitre.org/techniques/T1550/002/)|
|28|Scheduled Task FileAccess|[T1053.005](https://attack.mitre.org/techniques/T1053/005/)|
|29|Compiled HTML Access|[T1218.001](https://attack.mitre.org/techniques/T1218/001/)|
|30|Network Share Connection Removal|[T1070.005](https://attack.mitre.org/techniques/T1070/005/)|
|31|Local Network Sniffing|[T1040](https://attack.mitre.org/techniques/T1040/)|
|32|DLL Injection with Mavinject|[T1055.001]([T1055.001](https://attack.mitre.org/techniques/T1055/001/))|
|33|MSBuild and msxsl|[T1127](https://attack.mitre.org/techniques/T1127/)|
|34|Component Object Model Hijacking|[T1546.015](https://attack.mitre.org/techniques/T1546/015/)|
|35|CMSTP|[T1218.003](https://attack.mitre.org/techniques/T1218/003/)|
|36|Registry Edit from Screensaver|[T1546.002](https://attack.mitre.org/techniques/T1546/002/)|
|37|Credentials in Files & Registry|[T1552.002](https://attack.mitre.org/techniques/T1552/002/), [T1552.001](https://attack.mitre.org/techniques/T1552/001/)|
|38|AppInit DLLs|[T1546.010](https://attack.mitre.org/techniques/T1546/010/)|
|39|Clear Powershell Console Command History|[T1070.003](https://attack.mitre.org/techniques/T1070/003/)|
|40|Indicator Blocking - Driver Unloaded|[T1562.006](https://attack.mitre.org/techniques/T1562/006/)|
|41|Processes Started From Irregular Parent|[T1068](https://attack.mitre.org/techniques/T1068/)|
|42|Local Permission Group Discovery|[T1069.001](https://attack.mitre.org/techniques/T1069/001/)|
|43|Unusual Child Process for Spoolsv.Exe or Connhost.Exe|[T1068](https://attack.mitre.org/techniques/T1068/)|
|44|Unusual Child Process spawned using DDE exploit|[T1559.002](https://attack.mitre.org/techniques/T1559/002/)|
|45|Webshell-Indicative Process Tree|[T1505.003](https://attack.mitre.org/techniques/T1505/003/)|
|46|Detecting Tampering of Windows Defender Command Prompt|[T1562.001](https://attack.mitre.org/techniques/T1562/001/)|
|47|Identifying Port Scanning Activity|[T1046](https://attack.mitre.org/techniques/T1046/)|
|48|Disable UAC|[T1548.002](https://attack.mitre.org/techniques/T1548/002/)|
|49|Detecting Shadow Copy Deletion via Vssadmin.exe|[T1490](https://attack.mitre.org/techniques/T1490/)|
|50|Get System Elevation (Meterpreter and Cobalt Strike)|[T1548](https://attack.mitre.org/techniques/T1548/)|
|51|Get System Elevation (Empire and PoshC2)|[T1548](https://attack.mitre.org/techniques/T1548/)|
|52|Debuggers for Accessibility Applications|[T1546.012](https://attack.mitre.org/techniques/T1546/012/)|
|53|NTFS Alternate Data Stream Execution (powershell)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|54|NTFS Alternate Data Stream Execution (wmic)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|55|NTFS Alternate Data Stream Execution (rundll32)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|56|NTFS Alternate Data Stream Execution (wscript/cscript)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|57|NTFS Alternate Data Stream Execution (control)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|58|NTFS Alternate Data Stream Execution (appvlp)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|59|NTFS Alternate Data Stream Execution (cmd)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|60|NTFS Alternate Data Stream Execution (ftp)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|61|NTFS Alternate Data Stream Execution (bash)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|62|NTFS Alternate Data Stream Execution (mavinject)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|63|NTFS Alternate Data Stream Execution (bitsadmin)|[T1564.004](https://attack.mitre.org/techniques/T1564/004/)|
|64|Rare LolBAS Command Lines|[T1012](https://attack.mitre.org/techniques/T1012/), [T1112](https://attack.mitre.org/techniques/T1112/), [T1547](https://attack.mitre.org/techniques/T1547/), [T1574](https://attack.mitre.org/techniques/T1574/)|
|65|Unusually Long Command Line Strings|[T1059.003](https://attack.mitre.org/techniques/T1059/003/), [T1059.001](https://attack.mitre.org/techniques/T1059/001/)|



# Map to Local

Implementing rules based on [Techniques usage statistics](https://kooroshrz.github.io/MITRE-ATTACK/Statistics/)

## Command and Scripting Interpreter
+ [T1059](https://attack.mitre.org/techniques/T1059/)
+ [T1059.001](https://attack.mitre.org/techniques/T1059/001/)
+ [T1059.003](https://attack.mitre.org/techniques/T1059/003/)

### Rule number 13 (Powershell Execution) [T1059.001](https://attack.mitre.org/techniques/T1059/001/)

Severity : Medium

```
Processes.action=allowed
Processes.process_path = "C:\\Windows\\*\\powershell.exe"
Processes.parent_process_path != "C:\\Windows\\explorer.exe"

In last 24 hour
```


### Rule number 21 (Remote PowerShell Sessions) [T1059.001](https://attack.mitre.org/techniques/T1059/001/) T1021

Severity : Medium

```
Processes.process_exec = "wsmprovhost.exe"
Processes.parent_process_exec != "svchost.exe"

In last 24 hour
```


### Rule number 65 (Unusually Long Command Line Strings) [T1059.003](https://attack.mitre.org/techniques/T1059/003/), [T1059.001](https://attack.mitre.org/techniques/T1059/001/)

Severity : Low

```
max(process.length) > 10* average(process.length)

In last 24 hour
```

### Rule number 19 (Quick execution of a series of suspicious commands) T1087 T1003 T1069 T1057 T1021 T1543 T1112 T1574 T1018 T1569 T1053 T1029 T1033 T1007 T1082 T1049 T1016 T1010 T1518 T1046 T1562 T1098 T1059 T1012

Severity : Medium

```
Process.process_exec IN (“arp.exe", "at.exe", "attrib.exe", "cscript.exe",
"dsquery.exe", "hostname.exe", "ipconfig.exe", "mimikatz.exe", "nbstat.exe",
"net.exe", "netsh.exe", "nslookup.exe", "ping.exe", "quser.exe",
"qwinsta.exe", "reg.exe", "runas.exe", "sc.exe", "schtasks.exe",
"ssh.exe", "systeminfo.exe", "taskkill.exe", "telnet.exe", "tracert.exe",
"wscript.exe", "xcopy.exe”)
count(Process.process_exec) > 1

In last 24 hour
```


### Rule number 24 (Processes Spawning cmd.exe) [T1059.003](https://attack.mitre.org/techniques/T1059/003/)

Severity : Medium

```
Processes.process_exec = "cmd.exe"
Processes.parent_process_exec == "*"

In Last 24 hour
```


