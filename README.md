# Failed RDP to IP Geolocation Information

## Description

This is a demonstration of using Azure Sentinel to monitor failed RDP login attempts to a VM and present the geolocation data

This is achieved by parsing Windows event logs with powershell.  The IPs from the connection attempts are used to retrieve data from a geolocation API and the results are written to a custom log. The custom log is then queried by Sentinel and presented as an updated heatmap.

## Components

[Powershell Script](https://github.com/evasquez44/AzureSentinelLab/blob/main/Custom_Security_Log_Exporter.ps1)

[IP Geolocation API](https://ipgeolocation.io/)

[KQL Query](https://github.com/evasquez44/AzureSentinelLab/blob/main/Workbook%20Log%20Query)


## Attacks from Ukraine coming in; Custom logs being output with geodata

<img src="https://github.com/evasquez44/AzureSentinelLab/blob/main/Images/Incoming%20attacks.PNG" width="700">



## Worldmap of incoming attacks over time

<img src="https://github.com/evasquez44/AzureSentinelLab/blob/main/Images/Heatmap%20progression.png" width="700">
