📘 CHAPTER 1: INTRODUCTION TO .NET AND C#

Unit I – Introduction to .NET and C#
Beginner Friendly Notes | Flowcharts | Diagrams | Exam Preparation

🎯 Chapter Overview
                    ┌──────────────────────────┐
                    │   INTRODUCTION TO .NET   │
                    │          & C#            │
                    └────────────┬─────────────┘
                                 │
        ┌────────────────────────┼────────────────────────┐
        │                        │                        │
        ▼                        ▼                        ▼
      .NET                      CLR                       C#
        │                        │                        │
        ▼                        ▼                        ▼
 SDK / Runtime              IL + JIT              Program Structure
        │                        │                        │
        └────────────────────────┼────────────────────────┘
                                 │
                                 ▼
                         Build & Run Application
1️⃣ Introduction to .NET
What is .NET?

.NET is a software development platform developed by Microsoft.

.NET ka use different types ke applications banane aur run karne ke liye kiya jata hai.

.NET se kya bana sakte hain?
💻 Console Applications
🌐 Web Applications
🔌 Web APIs
🖥️ Desktop Applications
📱 Mobile Applications
☁️ Cloud Applications
🤖 IoT Applications
🎮 Games
Simple Flow
       👨‍💻 Developer writes C# Code
                    │
                    ▼
              ⚙️ .NET Platform
                    │
                    ▼
            🖥️ Application Runs
Easy Real-Life Analogy

Socho ek factory hai:

.NET Component	Real-Life Example
C#	Language used to give instructions
.NET	Complete factory/platform
SDK	Developer's toolbox
Runtime	Application chalane ka environment
CLR	Program chalane wala engine
Class Library	Ready-made tools
2️⃣ Features of .NET

.NET ki kuch important features hain.

1. Cross-Platform

Modern .NET applications multiple operating systems par run kar sakti hain.

        .NET APPLICATION
               │
      ┌────────┼────────┐
      ▼        ▼        ▼
   Windows   Linux    macOS
2. Multiple Language Support

.NET ecosystem multiple languages ko support karta hai.

Important languages:

C#
F#
Visual Basic .NET
3. Object-Oriented Programming

C# Object-Oriented Programming support karta hai.

Main OOP Concepts
             OOP
              │
    ┌─────────┼─────────┐
    ▼         ▼         ▼
Encapsulation Abstraction Inheritance
                         │
                         ▼
                    Polymorphism

In concepts ko Unit II mein detail mein padhenge.

4. Automatic Memory Management

.NET memory management mein Garbage Collector help karta hai.

Flowchart
Create Object
      │
      ▼
Object is Used
      │
      ▼
Object No Longer Needed
      │
      ▼
Garbage Collector
      │
      ▼
Memory Reclaimed
Simple Meaning

Programmer ko normally unused objects ki memory manually manage nahi karni padti.

5. Large Class Library

.NET mein bahut saari ready-made classes aur libraries available hoti hain.

Example:

Console.WriteLine("Hello World");

Aur:

int maximum = Math.Max(10, 20);

Console.WriteLine(maximum);

Output:

20

Humne maximum calculate karne ka complete algorithm khud nahi likha. Math class ready-made functionality provide karti hai.

3️⃣ .NET Framework vs .NET Core vs Modern .NET

Ye exam ke liye bahut important topic hai.

Evolution Flow
┌─────────────────┐
│ .NET Framework  │
│ Older platform  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│   .NET Core     │
│ Cross-platform  │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│   Modern .NET   │
│ Unified platform│
└─────────────────┘
Comparison
Feature	.NET Framework	.NET Core	Modern .NET
Platform	Mainly Windows	Cross-platform	Cross-platform
Performance	Traditional	Improved	Modern
Open Source	Older ecosystem	Yes	Yes
Usage	Legacy applications	Modern applications	Current development
Development	Older	Modern transition	Unified modern platform
Exam Definition

.NET Framework is the older Windows-focused implementation, .NET Core introduced modern cross-platform development, and modern .NET is the unified platform used for current application development.

4️⃣ .NET SDK vs Runtime

Ye dono concepts aksar confuse hote hain.

SDK
Full Form

SDK = Software Development Kit

SDK developers ke liye hota hai.

Iska use:

Project create karne ke liye
Code build karne ke liye
Compile karne ke liye
Application run karne ke liye
Testing ke liye
Publishing ke liye
Runtime

Runtime ka use mainly already developed application ko execute/run karne ke liye hota hai.

Flowchart
                DEVELOPER
                    │
                    ▼
              ┌──────────┐
              │   SDK    │
              └────┬─────┘
                   │
        ┌──────────┼──────────┐
        ▼          ▼          ▼
     Create      Build       Run
        │
        ▼
   Application
        │
        ▼
   ┌───────────┐
   │ Runtime   │
   └─────┬─────┘
         │
         ▼
 Application Runs
Difference
SDK	Runtime
Development ke liye	Application run karne ke liye
Create project	Run application
Build application	Execute application
Development tools provide karta hai	Runtime environment provide karta hai
Easy Trick 🔥

SDK = Develop + Build + Run

Runtime = Run

5️⃣ Common Language Runtime (CLR)
Full Form

CLR = Common Language Runtime

CLR .NET application ke execution environment ka important part hai.

CLR ke Main Functions
▶️ Code Execution
🧠 Memory Management
♻️ Garbage Collection
⚠️ Exception Handling
🔐 Runtime Security Services
⚙️ Execution Management
CLR Working
C# Program
    │
    ▼
Compilation
    │
    ▼
Intermediate Language (IL)
    │
    ▼
CLR
    │
    ▼
JIT Compilation
    │
    ▼
Machine Code
    │
    ▼
CPU Executes Program
6️⃣ Intermediate Language (IL)

C# code directly CPU language mein nahi likha jata.

Jab C# program compile hota hai, code intermediate form mein convert hota hai.

Isse kehte hain:

IL = Intermediate Language

Flow
C# Source Code
       │
       ▼
 C# Compiler
       │
       ▼
      IL
       │
       ▼
 CLR + JIT
       │
       ▼
 Machine Code
7️⃣ JIT Compiler
Full Form

JIT = Just-In-Time Compiler

JIT compiler IL instructions ko execution ke liye machine code mein convert karta hai.

Flowchart
        IL Code
           │
           ▼
     JIT Compiler
           │
           ▼
     Machine Code
           │
           ▼
          CPU
           │
           ▼
       Execution
⭐ MOST IMPORTANT: C# PROGRAM EXECUTION

Ye diagram exam mein bahut important hai.

┌──────────────────────┐
│ 1. Write C# Code     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 2. C# Compiler       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 3. IL Generated      │
│ Intermediate Language│
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 4. CLR Manages       │
│    Execution         │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 5. JIT Compiler      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 6. Machine Code      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 7. CPU Executes Code │
└──────────────────────┘
Short Answer

C# source code is compiled into Intermediate Language (IL). The CLR manages the execution of the program, and JIT compilation converts required IL into machine code so that the CPU can execute it.

8️⃣ .NET Class Library

.NET mein bahut saari pre-written classes available hoti hain.

In classes ka use karke hum application fast develop kar sakte hain.

Example
Console.WriteLine("Hello");

double answer = Math.Sqrt(25);

Console.WriteLine(answer);

Output:

Hello
5
Important Namespaces
System
using System;

Basic functionality provide karta hai.

System.Collections.Generic
using System.Collections.Generic;

Collections ke liye.

System.IO
using System.IO;

Files aur input/output operations ke liye.

9️⃣ Development Environment

.NET aur C# programming ke liye mainly do environments use kiye ja sakte hain.

🖥️ Visual Studio

Visual Studio ek full-featured IDE hai.

IDE Full Form

Integrated Development Environment

Features
Code Editor
Debugger
IntelliSense
Project Management
Git Integration
GUI Tools
💻 Visual Studio Code

VS Code ek lightweight aur extensible code editor hai.

Features
Lightweight
Fast
Cross-platform
Extensions
Terminal Integration
Comparison
Visual Studio	VS Code
Full IDE	Lightweight editor
More built-in tools	Extension-based
Large installation	Smaller installation
GUI development support	Flexible development
🔟 .NET CLI
Full Form

CLI = Command Line Interface

.NET CLI ka use terminal ya command prompt se .NET projects manage karne ke liye hota hai.

Important CLI Commands 🔥
Check .NET Version
dotnet --version
Create Console Application
dotnet new console
Create Project with Name
dotnet new console -n MyApp
Open Project Folder
cd MyApp
Run Application
dotnet run
Build Application
dotnet build
Restore Dependencies
dotnet restore
Add NuGet Package
dotnet add package PackageName

Example:

dotnet add package Newtonsoft.Json
Complete CLI Workflow
dotnet new console -n MyApp
             │
             ▼
          cd MyApp
             │
             ▼
        Write Code
             │
             ▼
        dotnet build
             │
             ▼
         dotnet run
             │
             ▼
       Program Output
1️⃣1️⃣ Project Structure in .NET

Jab hum new project create karte hain:

dotnet new console -n MyApp

To typical project structure:

MyApp/
│
├── Program.cs
├── MyApp.csproj
│
├── bin/
│
└── obj/
Program.cs

Main source code file.

Example:

Console.WriteLine("Hello World");
.csproj File

Project configuration file hoti hai.

Isme information ho sakti hai:

Target Framework
Project Settings
Package References
Build Configuration
bin Folder

Build output generally yahan generate hota hai.

obj Folder

Build ke intermediate files yahan generate hote hain.

1️⃣2️⃣ NuGet Package Manager

NuGet .NET ecosystem ka package manager hai.

Package kya hota hai?

Package reusable functionality provide karta hai.

Instead of everything from scratch:

Need Functionality
       │
       ▼
Search NuGet Package
       │
       ▼
Install Package
       │
       ▼
Use in Project
CLI se Package Install
dotnet add package PackageName
1️⃣3️⃣ Building and Executing .NET Application
Build
dotnet build
Build Flow
Source Code
    │
    ▼
Compiler Checks Code
    │
    ▼
Errors / Warnings
    │
    ▼
Build Output Generated
Run
dotnet run
Run Flow
Build
  │
  ▼
Execute Application
  │
  ▼
Display Output
1️⃣4️⃣ Introduction to C#

C# ko pronounce karte hain:

C Sharp

C# ek modern programming language hai jo .NET ecosystem mein extensively use hoti hai.

Features
Object-Oriented
Strongly Typed
Modern
.NET Applications ke liye use hoti hai
1️⃣5️⃣ C# Program Structure
Modern C# Program
Console.WriteLine("Hello World");
Traditional Program Structure
using System;

namespace MyApplication
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World");
        }
    }
}
Explanation
using System;

System namespace ke classes/types ko conveniently access karne mein help karta hai.

namespace MyApplication

Related code ko logically organize karta hai.

class Program

Program class define karta hai.

static void Main(string[] args)

Traditional C# program entry point.

Console.WriteLine()

Console screen par output print karta hai.

1️⃣6️⃣ Hello World Program
Console.WriteLine("Hello World");

Output:

Hello World
1️⃣7️⃣ Introduction to Git
Git kya hai?

Git ek:

Version Control System

hai.

Git source code mein hone wale changes ko track karta hai.

Why Git?
Version 1
   │
   ▼
Version 2
   │
   ▼
Version 3
   │
   ▼
Bug / Problem
   │
   ▼
Previous Version Check

Git help karta hai:

Kya change hua?
Kab change hua?
Kis commit mein change hua?
Important Git Commands
Initialize Repository
git init
Check Status
git status
Add Files
git add .
Commit Changes
git commit -m "Initial commit"
View Commit History
git log
1️⃣8️⃣ GitHub

GitHub ek online platform hai jahan Git repositories host ki ja sakti hain.

Workflow
👨‍💻 Write Code
       │
       ▼
     Git
       │
       ▼
 Local Repository
       │
       ▼
    git push
       │
       ▼
 ☁️ GitHub Repository
