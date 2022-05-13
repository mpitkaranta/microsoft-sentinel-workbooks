# Introduction
This repository contains workbooks I've developed for Microsoft Sentinel. Some of them are based on Microsoft templates. Enjoy!

# Workbooks

## Server agent status
Server agent status workbook displays information about various security agents installed on your servers (both ARC servers and virtual machines).

To use the workbook, simply set the subscription and workspace to point into your Sentinel workspace.

![Workspace parameters](/Images/WorkspaceParameters.png)

Optionally, you can modify the **DefaultSubscription_Internal** and **DefaultWorkspace_Internal** parameters to permanently store the workspace information into the workbook (you need to be in edit mode to set the parameters). This way, anyone opening the workbook for the first time will have the correct workspace selected by default. 

![Workspace default parameters](/Images/WorkspaceDefaultParameters.png)

Once the parameters have been set, click **Load data** to load the data. 

You can change the the parameters to filter out the results, or to change the definition of "unhealthy" (if heartbeats are not found within the timeframe -> unhealthy). 

![Server agent status](/Images/ServerParameters.png)

The workbook will display status information from different agents. Hovering your mouse over the status will display additional information (in the example below, the timestamp of the last event received).

![Server agent status](/Images/ServerAgentStatus.png)


