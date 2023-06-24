---
title: Lesson 1
subtitle: Powershell versions
layout: page
hide_hero: false
show_sidebar: false
---
## Powershell versions
Powershell version is devided in to tow sections
* Windows Powershell
* Powershell Core

### Windows Powershell
Powershell on windows can be install on Server 2008 and above ( you sould upgrade to newer server :) )\
Server 2016 and above have the Version 5.1, no more upgrades for Windows Powershell.

### Powershell Core
Powershell core is the ongoing version we use.
We can install the Powershell Core on Windows or Linux.\
Currently the Powershell Core version is 7.x (you can see the actual version in [Powershell Github](https://github.com/PowerShell/PowerShell))

### Install Powershell
Use the [Powershell Github](https://github.com/PowerShell/PowerShell) To install Powershell 7 on your system.\
Powershell Core and Microsoft Powershell can both run on the same system.

### Windows Powershell
Everything we learn we can do with Windows Powershell 5.1

### Get Powershell Version
We work with ISE (Integrated Scripting Environment) is the environment where we wright our scripts, it also called IDE\
![image](https://github.com/itamartz/Powershell/assets/10198823/cbde8727-1dbf-4744-b58e-9f71b1cbd95f)\
In the bottom of the screen in the blue section put this code.

```powershell
$PSVersionTable
```
![image](https://github.com/itamartz/Powershell/assets/10198823/b087fda1-5ab5-4f0f-a8c4-5544e754dfe6)\
The PSVersion is your Windows Powershell Version

