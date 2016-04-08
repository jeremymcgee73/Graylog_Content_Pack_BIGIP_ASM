# F5 Big-IP ASM Content Pack
This content pack is used to capture log data from F5's Big-IP Application Security Module.

## Includes
* Input (Syslog TCP 1514)

##TO DO
I have just started working on this. I have been struggling to get ASM's logs into Graylog for awhile. I finaly sat down and learned GROK filters. I really shouldn't be using the DATA grok pattern for all fields.

##Logging Profile
A logging profile will have to be created. Then you will have to select the logging profile on the virtual servers that you are wanting. I have included a screenshot of my logging profile for reference.

Import Logging Profile Settings:
* "Protocol" set to "TCP"
* "Remote Storage Type" set to "Reporting Server"
* "Server Address" set to "graylogserver:1514"

![Alt text](/images/logging_profile.png?raw=true "Logging Profile")
