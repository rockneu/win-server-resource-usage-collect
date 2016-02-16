win-server-resource-usage-collect
=================================

windows server resource usage collection.
This set of scripts is used to collect windows server system resource consuming info(cpu, mem, disk).

If to get localhost's resource consuming info, just run script getInfo.bat, and getInfo.bat will call getResc.vbs to get resource data. 

If to get other windows nodes' info, need to copy file getInfo.bat & getResc.vbs to the windows nodes' %windir%\system32. Then run the tool psexec locally to connect to remote windows nodes, and then view the desired info at psexec console.

1 Precondition:
If to view other windows hosts' resource consuming info, need to copy getInfo.bat and getResc.vbs to those hosts at directory %windir%\system32\.


2.Usage:
2.1 to get the resource info from localhost,just run getInfo.bat;
2.2 to get the resource info from the server list(srvlist.txt) at LAN ENV(pstools needed), start psexec just run runScript.bat


3.File introduction:
getInfo.bat
	--show windows system resource usage info, including cpu, memory, and disk usage info.

getResc.vbs
	--the real one to get windows resource consumption info, and it's called by getInfo.bat.

srvlist.txt
	--list the server list to get resource usage info.

