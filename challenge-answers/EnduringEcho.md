**What was the first (non cd) command executed by the attacker on the host? (string)**
systeminfo

**Which parent process (full path) spawned the attacker’s commands? (C:\FOLDER\PATH\FILE.ext)**
C:\Windows\System32\wbem\WmiPrvSE.exe

**Which remote-execution tool was most likely used for the attack? (filename.ext)**
wmiexec.py

**What was the attacker’s IP address? (IPv4 address)**
10.129.242.110

**What is the first element in the attacker's sequence of persistence mechanisms? (string)**
SysHelper Update

**Identify the script executed by the persistence mechanism. (C:\FOLDER\PATH\FILE.ext)**
C:\Users\Werni\AppData\Local\JM.ps1

**What local account did the attacker create? (string)**
svc_netupd

**What domain name did the attacker use for credential exfiltration? (domain)**
NapoleonsBlackPearl.htb

**What password did the attacker's script generate for the newly created user? (string)**
Watson_20250824160509

**What was the IP address of the internal system the attacker pivoted to? (IPv4 address)**
192.168.1.101

**Which TCP port on the victim was forwarded to enable the pivot? (port 0-65565)**
9999

**What is the full registry path that stores persistent IPv4→IPv4 TCP listener-to-target mappings? (HKLM\...\...)**
HKLM\SYSTEM\CurrentControlSet\Services\PortProxy\v4tov4\tcp

**What is the MITRE ATT&CK ID associated with the previous technique used by the attacker to pivot to the internal system? (Txxxx.xxx)**
T1090.001

**Before the attack, the administrator configured Windows to capture command line details in the event logs. What command did they run to achieve this? (command)**
reg add "HKLM\Software\Microsoft\Windows\CurrentVersion\Policies\System\Audit" /v ProcessCreationIncludeCmdLine_Enabled /t REG_DWORD /d 1 /f
