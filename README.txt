win-server-resource-usage-collect
=================================

windows server resource usage collection.

1 Precondition:
1.1 This set of scripts is used to collect windows server system resource consuming info(cpu, mem, disk).
1.2 It needs free tool PSTools(a free "ssh" tool on windows platform from MS staff) to cooperate with.


2.Usage:
2.1 to get the resource info from localhost,just run getInfo.bat;
2.2 to get the resource info from the server list(srvlist.txt) at LAN ENV( precondition1.2 should be met), start psexec just run runScript.bat


3.File introduction:
getInfo.bat
	--show windows system resource usage info, including cpu, memory, and disk usage info.

getResc.vbs
	--the real one to get windows resource consumption info, and it's called by getInfo.bat.

srvlist.txt
	--list the server list to get resource usage info.

