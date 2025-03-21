# Microsoft Windows [Version 10.0.26100.3476]
(c) Microsoft Corporation. All rights reserved.

C:\work>wmic cpu get caption, name, deviceid, numberofcores, maxclockspeed, status
Caption                                DeviceID  MaxClockSpeed  Name                                 NumberOfCores  Status
Intel64 Family 6 Model 183 Stepping 1  CPU0      2100           13th Gen Intel(R) Core(TM) i7-13700  16             OK  


C:\work>

## 3 sites that explain what WMIC command is about.

(https://learn.microsoft.com/en-us/windows/win32/wmisdk/wmic)

The WMI command-line (WMIC) utility provides a command-line interface for Windows Management Instrumentation (WMI). WMIC is compatible with existing shells and utility commands. The following information is a general

reference guide for WMIC. For more information and guidelines on how to use WMIC, including additional information on aliases, verbs, switches, and commands, see Using Windows Management Instrumentation command-line and WMIC

Take command-line control over WMI.

(https://askgarth.com/blog/how-to-use-wmic/)

 I talked about using Windows Management Instrumentation Command-line (WMIC) to troubleshoot WMI issues. I need to user WMIC to troubleshoot a x86 problem on a x64 computer. You might think that Wbemtest would be the tool to use but on a x64 computer there is no x86 version of webemtest on those computers. You might be wondering about how to use WMIC for similar issues, so I thought that I would share the steps I take.
 
(https://medium.com/@nirvana.elahi/wmic-risks-threats-and-detection-techniques-f287a4488167)

