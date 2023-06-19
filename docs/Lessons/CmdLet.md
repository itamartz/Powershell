---
title: CmdLet
subtitle: Powershell CmdLet
layout: page
hide_hero: false
show_sidebar: false
---
## CmdLet
In Powershell the command call CmdLet, this is a command that create using dot net.

In Powershell, we can create 2 type of command
* CmdLet - using Dot Net
* function - using Powershell

If we run the Cmdlet Get-Command we can get the list of all the CmdLet / function we have on our system
```powershell
Get-Command
```
![image](https://github.com/itamartz/Powershell/assets/10198823/60c64a00-0566-43b4-880a-b3f7d44fa95d)

And if I run this command I can group all the type of commands I have in my system
```powershell
Get-Command | Group-Object -Property CommandType
```
![image](https://github.com/itamartz/Powershell/assets/10198823/36b2b031-7cba-4018-9d34-69748ed61580)
