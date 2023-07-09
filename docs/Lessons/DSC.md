---
title: (D)esired (S)tate (C)onfiguration
subtitle: Powershell DSC
layout: page
hide_hero: false
show_sidebar: false
---

## (D)esired (S)tate (C)onfiguration [DSC](https://learn.microsoft.com/en-us/powershell/dsc/getting-started/wingettingstarted)
After we create our script to do something the next step is to declare what we want and lets the System (Powershell) to decide how to do what we want.

# Example
Lets say we want to create a new Datacenter, if we use PowerCli we need to use this code

```powershell
$folder = Get-Folder -NoRecursion | New-Folder -Name Folder
    
New-Datacenter -Location $folder -Name Datacenter_Haifa
```
If we use the DSC the code can look like this:
```powershell
Configuration vCenter_Config {

  Datacenter "PoShDSC_DC" {
      Server = $Server
      Credential = $VcCreds
      Name = 'Datacenter_Haifa'    
      Location = [string]::Empty
      Ensure = 'Present'
  }
}

Start-DscConfiguration vCenter_Config
```
This code declare what we want, and the System figure out how to create this configuration. (this code is from Internet, not test)

**Ansible** also work like this.
