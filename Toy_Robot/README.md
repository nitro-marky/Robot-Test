﻿# Toy Robot - Mark Addis 

This guide explains how to test the Toy Robot simulator using the provided test files and custom files.
This has been written in C# .NET 8.0

### Requirements
.NET 8.0 SDK installed

*Not 100% necessary as you can run `dotnet run` - Build Project (`dotnet build`)*

Test Files Included
The project includes two test files in the root directory:<br>

robot-test.txt - Basic functionality tests prodivded with the brief<br>
robot-test2.txt - Comprehensive in-depth testing

## Testing Methods - All these methods should use a command prompt opened in Toy_Robot Folder
### Method 1: Using Provided Test Files

Quick Test - Open a console window in the project folder (Toy_Robot) 

`dotnet run -- robot-test.txt`

Comprehensive Test (In-Depth)

`dotnet run -- robot-test2.txt`

### Method 2: Custom Test Files
Create your own test file and run it:<br>
`dotnet run -- "C:\Code\Toy Robot\Toy_Robot\myTests.txt"` For example.

## Running Automated Tests

Execute the automated test suite (the test folder must be in the same root folder as the project):<br>
`dotnet test`

---
### How the table is layed out
Y<br>
4  [ ][ ][ ][ ][ ]  ← NORTH edge<br>
3  [ ][ ][ ][ ][ ]<br>
2  [ ][ ][ ][ ][ ]<br>
1  [ ][ ][ ][ ][ ]<br>
0  [0][ ][ ][ ][4]  ← SOUTH edge (Y=0)<br>
   0  1  2  3  4 -  X<br>
   ↑---------             ↑<br>
 WEST---            EAST<br>
 edge----            edge<br>
