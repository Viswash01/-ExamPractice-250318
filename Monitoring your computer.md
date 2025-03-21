# 1 Using Task Manager to Monitor Server Performance

Task Manager provides a high-level overview of the system's performance. Here's how to use it:

Open Task Manager:

Press Ctrl + Shift + Esc or right-click the taskbar and select Task Manager.

## Key Tabs in Task Manager:

Processes: Shows the running applications and background processes. You can monitor the CPU, memory, disk, and network usage for each process.

Right-click a process to end it, view details, or set priority.

Sort the processes by resource usage (CPU, Memory, Disk, or Network).

Performance: Provides a detailed view of resource usage on your server.

CPU: Displays the overall CPU usage, usage by individual cores, and details like the current clock speed and the number of processes running.

Memory: Displays the RAM usage, including total used memory, available memory, and the committed memory.

Disk: Shows the read/write activity on the disk, which helps to identify bottlenecks.

Network: Displays network usage and helps you monitor how much data is being sent and received by your server.

App History: Shows resource usage over time for apps that are running. This is useful for spotting performance patterns.

## How to Monitor:

To monitor the server’s overall performance, check the Performance tab for real-time graphs of CPU, memory, disk, and network usage.

To find problematic processes, go to the Processes tab and look for any processes that are consuming excessive resources.

# Using Resource Monitor to Monitor Server Performance

Resource Monitor gives a more detailed and granular view of the system's resource usage compared to Task Manager.

Open Resource Monitor:

From Task Manager (under the Performance tab), click on Open Resource Monitor at the bottom.

Alternatively, press Windows + R, type resmon, and press Enter.

## Key Sections in Resource Monitor:

CPU: Provides detailed information about CPU usage, including which processes are using the CPU, and their individual threads. It also shows the average CPU usage and the CPU frequency.

You can also see CPU usage by individual processes, and whether any process is causing high CPU load.

Associated Handles: Lists all open handles by processes and the specific files, folders, or services they are using.

Memory: Shows detailed memory usage and splits it into categories such as:


Hard Faults/sec: Indicates memory paging.

Commit (MB): Shows the committed memory usage.

Private (MB): Displays how much memory a process is using that cannot be shared.

Disk: Displays real-time data about disk usage, including processes that are reading or writing to disk, and the amount of data being transferred.

You can see disk queue lengths, read/write speeds, and processes involved in disk activity.

Network: Shows detailed network usage, including the processes and services that are using network resources.

You can monitor the total network activity and the data being sent and received by your server.

TCP Connections: Lists all active network connections and associated processes, helpful for identifying any network bottlenecks.

# 2 How to Identify Bottlenecks:

High Memory Usage: If your server is constantly using most of its available memory, it could be an issue of insufficient RAM or poor memory management in certain applications.

Paging: If Hard Faults/sec is consistently high, it indicates that your server is paging, which occurs when physical RAM is full and data is being swapped to disk. This leads to significant performance degradation.

Memory Leaks: Check for processes that are consuming large amounts of memory without releasing it. In Resource Monitor, the Private (MB) column can help you spot these.Monitoring Network Utilization
Network bottlenecks can result from high data transfer, leading to slow communication and delays.

## Steps in Task Manager:

In Task Manager, go to the Performance tab and check Network usage. If your network utilization is consistently high (near 100%), this may indicate network congestion.

Steps in Resource Monitor:

In Resource Monitor, go to the Network tab to see detailed information on data sent/received by processes.

Check the Network Activity section to see which processes are using the most network resources.

Pay attention to the TCP Connections section to see the active connections and their statuses.

How to Identify Bottlenecks:

High Network Utilization: If the server is consuming excessive bandwidth (above 80-90% of the network capacity), this could indicate network congestion, which will cause slowdowns in data transmission. Identify processes that are using the network and evaluate whether they are necessary or need optimization.

Excessive Open Connections: If you notice a large number of open connections, it could indicate a misconfigured application or an issue with the network stack.

# There are 3 websites that have how to procedure of how to Monitorythe function of your computer

(https://www.hp.com/us-en/shop/tech-takes/how-to-monitor-your-computers-performance)

(https://www.insightful.io/blog/how-to-track-computer-activity)

(https://www.timedoctor.com/blog/what-is-computer-monitoring/)
