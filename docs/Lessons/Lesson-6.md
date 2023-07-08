---
title: Lesson 6
subtitle: Powershell Loop
layout: page
hide_hero: false
show_sidebar: false
---
## What is a Loop
A loop is using when you have more then one object that you want to work on.\
For example when we run the CmdLet Get-Service we get a array of service objects.

```powershell
$AllServices = Get-Service
```
We can walk over the services we have on our computer using loop.

## List of loop
* For
* Foreach
* while
* do

Usually if we have an array of object we want to loop them using **foreach**.

```powershell
$AllServices = Get-Service
foreach($item in $AllServices)
{
    $item
}
```
Lets explain this loop, the $item is the variable that get the current object in the array.

On the first loop the $item point on the first object in the array.
```powershell
  $item
[service][service][service]

```

On the second loop the $item point on the second object in the array.
```powershell
           $item
[service][service][service]

```

If we want to loop over the 10 first items in the loop, we can use **for**.
```powershell
$AllServices = Get-Service
for($i; $i -lt $AllServicesLength; $i++)
{
    $AllServices[$i]
}
```
Lets explain this loop, the $item is the variable that get the current object in the array.
the **-lt** is operator in powershell for less then

On the first loop the $i point on the first object in the array ($i=0).
```powershell
  [$i]
[service] [service] [service]

```
On the second loop the $i point on the second object in the array ($i=1).
```powershell
           [$i]
[service][service][service]

```

If we want to delay the next command until we have the correct data we can use **While**.
```powershell

$i = 0
while($i -lt 10)
{
    $i++
}
```
Lets explain this loop, the $i is the variable that get the current number, the ++ is a short for
```powershell
$i = $i + 1
```

If we want to start a loop and then check for the data we can use the **do**.

```powershell
do
{
  $ip = Read-Host 'Enter IPv4:'
} while ($ip -notlike '*.*.*.*')

```
Lets explain this loop, the $ip is the variable that get form user the ip address, and the loop stop if the $ip is not a IP address.\
The -notlike is a operator in Powershell for regex.\
If the text we got from the $IP is not like text . text . text . text is stop the loop.\
This example not check if the $ip is an actual IP Address.

## Example for loops
In the Powershell website we have a lot of example so look there.
* [For](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_for)
* [Foreach](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_foreach)
* [While](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_while)
* [Do](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_do)