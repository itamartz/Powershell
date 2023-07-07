---
title: Lesson 2
subtitle: Powershell Help
layout: page
hide_hero: false
show_sidebar: false
---
## Powershell Help
Powershell help is a powerful tools, it's lets you the option to search the command you want, what parameters the function need etc..

## Help versions
In the begging of Powershell, we have help with our module, CmdLet.\
Starting from version 3 Microsoft decide to separate the help from the module, this separations give as the ability to fix the help and not the module, servers does not have help etc..

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

## Using Powershell Help
Lets search command to restart computer.
we using the help  command like so

```powershell
help *restart*
```

This will return the result of all command that have the restart in there help Or in the Cmdlet name

![image](https://github.com/itamartz/Powershell/assets/10198823/b1af4a34-ff98-4dd9-bbbb-c37561293d2a)

