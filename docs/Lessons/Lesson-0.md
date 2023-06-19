---
title: Lesson 0
subtitle: Before we start with Powershell
layout: page
hide_hero: false
show_sidebar: false
---
## Object Oriented Programming - OOP
Before we can start learn the Powershell language, we need to learn the basic.

(OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. 
An object can be defined as a data field that has unique attributes and behavior.

## Explain OOP in a example

Car -> is of type object of a Car.
Object is a Instance of the Class.
Class is the Blue print

Powershell is a language writing in dot net so I will write the example in a C#.

```cs
public class Car
{
    public int Speed { get; set; }
    public string Model { get; set; }
}
```
And if I want to create a Object from this blue print.
```cs
Car Tesla = new Car();
```
And if I want to get model from this Car object

```cs
Tesla.Model
'''

this is in a nutshell dot net.

### Powershell return Object(s) so you can use the OOB to deal with the result of running a CmdLet in Powershell
