# Azure Sentinel Lab

## Description

This is a demonstration of using Azure Sentinel to monitor and present failed RDP login attempts via geolocation.

This is achieved by parsing Windows event logs with a powershell script.  The script feeds the results to a geolocation API and writes the results to a custom log. The custom log is then queried by Sentinel and presented as a heatmap that is updated automatically.
