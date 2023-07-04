---
title: Lesson 2
subtitle: Powershell Help
layout: page
hide_hero: false
show_sidebar: false
---
## Powershell Help
Powershell help is a powerfull tools, it's lets you the option to search the command you want, what parameters the function need etc..

## Help versions
In the begging of Powershell, we have help with our module, CmdLet.\
Starting from version 3 Microsoft decide to seperate the help from the module, this seperations give as the ability to fix the help and not the module, servers does not have help etc..

Powershell 5.1 (the last version of Windows Powershell) does not have help to the modules in the Microsoft server, you need to install the help on your local computer.

## Update help local
Open your ISE and type the CmdLet Update-Help and run this CmdLet using the F5

```powershell
Update-Help
```

This will trigger the downloads of all the help file for your module in your computer.

## Update help offline
On computer who connect to the internet, run this CmdLet
```powershell
Save-Help -DestinationPath C:\temp\OfflineUpdates
```

On the Offline computer you should run this command
```powershell
Update-Help -SourcePath C:\temp\OfflineUpdates
```