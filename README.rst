EvtxtoElk
============

A lightweight tool to load Windows Event Log evtx files into Elasticsearch.

Examples
--------

Blog is initially avaliable here: https://web.archive.org/web/20221209023101/https://www.dragos.com/blog/industry-news/evtxtoelk-a-python-module-to-load-windows-event-logs-into-elasticsearch/

I have now updated this script a bit. It now can parse folders or single files correctly. Also, now it will succeed in parsing timestamps from sysmon logs. Please let me know if there are any errors when using it. Email me at nathan@nathan2.com. 

Usage: 
python3 evtxtoelk.py ~/Downloads/ http://elastic:password@ip:9200  -i unit42

Downloads is the folder with evtx files to parse. You can also point at a single file. 
Change the password and ip to match your instance. 
i is the index. By default, it will upload to hostlogs if not specified.


