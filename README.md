# Azure Sentinel Lab

## Description

This is a demonstration of using Azure Sentinel to monitor failed RDP login attempts and present the geolocation data

This is achieved by parsing Windows event logs using a powershell script.  The script feeds the results to a geolocation API and writes the results to a custom log. The custom log is then queried by Sentinel and presented as a heatmap that is updated automatically.

## Components

[Powershell Script](http://mylink)

[IP Geolocation API](https://ipgeolocation.io/)
