---
title: Visual Studio Community 2022 workload and component IDs
titleSuffix: ""
description: "Use workload and component IDs to install Visual Studio by using the command line or to specify as a dependency in a VSIX manifest"
keywords:
author: anandmeg
ms.author: meghaanand
manager: jmartens
ms.date: 11/08/2022
ms.prod: visual-studio-windows
ms.technology: vs-installation
ms.topic: include
---
## Visual Studio core editor (included with Visual Studio Community 2022)

**ID:** Microsoft.VisualStudio.Workload.CoreEditor

**Description:** The Visual Studio core shell experience, including syntax-aware code editing, source code control and work item management.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.VisualStudio.Component.CoreEditor | Visual Studio core editor | 17.4.33006.217 | Required

## Azure development

**ID:** Microsoft.VisualStudio.Workload.Azure

**Description:** Azure SDKs, tools, and projects for developing cloud apps and creating resources using .NET and .NET Framework. Also includes tools for containerizing your application, including Docker support.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Component.Microsoft.VisualStudio.RazorExtension | Razor Language Services | 17.4.33006.217 | Required
Component.Microsoft.VisualStudio.Web.AzureFunctions | Azure WebJobs Tools | 17.4.33006.217 | Required
Component.Microsoft.Web.LibraryManager | Library Manager | 17.4.33006.217 | Required
Component.Microsoft.WebTools.BrowserLink.WebLivePreview | Web Live Preview | 17.4.51.37770 | Required
Microsoft.Component.ClickOnce | ClickOnce Publishing | 17.4.33006.217 | Required
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.ComponentGroup.ClickOnce.Publish | ClickOnce Publishing for .NET  | 17.4.33015.44 | Required
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Required
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Required
Microsoft.NetCore.Component.DevelopmentTools | Development tools for .NET | 17.4.33006.217 | Required
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Required
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Web | Web development tools for .NET | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Azure.ClientLibs | Azure libraries for .NET | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.DockerTools | Container development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.FSharp | F# language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.FSharp.WebTemplates | F# language support for web projects | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.IISExpress | IIS Express  | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.ManagedDesktop.Core | Managed Desktop Workload Core | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MSODBC.SQL | SQL Server ODBC Driver | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MSSQL.CMDLnUtils | SQL Server Command Line Utilities | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.DataSources | Data sources for SQL Server support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.LocalDB.Runtime | SQL Server Express 2019 LocalDB | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.SSDT | SQL Server Data Tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Azure.Prerequisites | Azure development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.AzureFunctions | Azure WebJobs Tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Required
Microsoft.Component.Azure.DataLake.Tools | Azure Data Lake and Stream Analytics Tools | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.TargetingPack | .NET Framework 4.8 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.4.8.DeveloperTools | .NET Framework 4.8 development tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.AuthoringTools | Azure Authoring Tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.Compute.Emulator | Azure Compute Emulator | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.Powershell | Azure Powershell | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.ResourceManager.Tools | Azure Resource Manager core tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.ServiceFabric.Tools | Service Fabric Tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.Waverton | Azure Cloud Services core tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Azure.Waverton.BuildTools | Azure Cloud Services build tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.DiagnosticTools | .NET profiling tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.Azure.CloudServices | Azure Cloud Services tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.Azure.ResourceManager.Tools | Azure Resource Manager tools | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.6.2.TargetingPack | .NET Framework 4.6.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.1.TargetingPack | .NET Framework 4.7.1 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.TargetingPack | .NET Framework 4.7 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.1.SDK | .NET Framework 4.8.1 SDK | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.1.TargetingPack | .NET Framework 4.8.1 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.4.6.2-4.7.1.DeveloperTools | .NET Framework 4.6.2-4.7.1 development tools | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.4.8.1.DeveloperTools | .NET Framework 4.8.1 development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.AspNet | .NET Framework project and item templates | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.AspNet45 | Advanced ASP.NET features | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Wcf.Tooling | Windows Communication Foundation | 17.4.33006.217 | Optional

## Data storage and processing

**ID:** Microsoft.VisualStudio.Workload.Data

**Description:** Connect, develop, and test data solutions with SQL Server, Azure Data Lake, or Hadoop.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.Azure.DataLake.Tools | Azure Data Lake and Stream Analytics Tools | 17.4.33006.217 | Recommended
Microsoft.Component.ClickOnce | ClickOnce Publishing | 17.4.33006.217 | Recommended
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.ManagedDesktop.Core | Managed Desktop Workload Core | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.MSODBC.SQL | SQL Server ODBC Driver | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.MSSQL.CMDLnUtils | SQL Server Command Line Utilities | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.SQL.LocalDB.Runtime | SQL Server Express 2019 LocalDB | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.SQL.SSDT | SQL Server Data Tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.FSharp.Desktop | F# desktop language support | 17.4.33006.217 | Optional

## Data science and analytical applications

**ID:** Microsoft.VisualStudio.Workload.DataScience

**Description:** Languages and tooling for creating data science applications, including Python and F#.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.PythonTools | Python language support | 17.4.33006.217 | Recommended
Microsoft.Component.PythonTools.Web | Python web support | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.FSharp.Desktop | F# desktop language support | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Recommended
Microsoft.ComponentGroup.PythonTools.NativeDevelopment | Python native development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Graphics.Tools | Graphics debugger and GPU profiler for DirectX | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.DiagnosticTools | C++ profiling tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK | Windows Universal C Runtime | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows11SDK.22000 | Windows 11 SDK (10.0.22000.0) | 17.4.33006.217 | Optional

## .NET desktop development

**ID:** Microsoft.VisualStudio.Workload.ManagedDesktop

**Description:** Build WPF, Windows Forms, and console applications using C#, Visual Basic, and F# with .NET and .NET Framework.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.ClickOnce | ClickOnce Publishing | 17.4.33006.217 | Required
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Required
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Required
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Required
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Required
Microsoft.VisualStudio.Component.ManagedDesktop.Core | Managed Desktop Workload Core | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.ManagedDesktop.Prerequisites | .NET desktop development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Required
Component.Microsoft.VisualStudio.LiveShare.2022 | Live Share | 1.0.5716 | Recommended
Microsoft.ComponentGroup.Blend | Blend for Visual Studio | 17.4.33006.217 | Recommended
Microsoft.ComponentGroup.ClickOnce.Publish | ClickOnce Publishing for .NET  | 17.4.33015.44 | Recommended
Microsoft.Net.Component.4.8.1.SDK | .NET Framework 4.8.1 SDK | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.1.TargetingPack | .NET Framework 4.8.1 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.TargetingPack | .NET Framework 4.8 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.4.8.1.DeveloperTools | .NET Framework 4.8.1 development tools | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.4.8.DeveloperTools | .NET Framework 4.8 development tools | 17.4.33006.217 | Recommended
Microsoft.NetCore.Component.DevelopmentTools | Development tools for .NET | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Debugger.JustInTime | Just-In-Time debugger | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.DiagnosticTools | .NET profiling tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.DotNetModelBuilder | ML.NET Model Builder | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.EntityFramework | Entity Framework 6 tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.FSharp | F# language support | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Recommended
Component.Dotfuscator | PreEmptive Protection - Dotfuscator | 17.4.33006.217 | Optional
Component.Microsoft.VisualStudio.RazorExtension | Razor Language Services | 17.4.33006.217 | Optional
Component.Microsoft.Web.LibraryManager | Library Manager | 17.4.33006.217 | Optional
Component.Microsoft.WebTools.BrowserLink.WebLivePreview | Web Live Preview | 17.4.51.37770 | Optional
Microsoft.Net.Component.4.6.2.TargetingPack | .NET Framework 4.6.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.1.TargetingPack | .NET Framework 4.7.1 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.TargetingPack | .NET Framework 4.7 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.4.6.2-4.7.1.DeveloperTools | .NET Framework 4.6.2-4.7.1 development tools | 17.4.33006.217 | Optional
Microsoft.NetCore.Component.Web | Web development tools for .NET | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.DockerTools | Container development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.FSharp.Desktop | F# desktop language support | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.FSharp.WebTemplates | F# language support for web projects | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.IISExpress | IIS Express  | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.MSODBC.SQL | SQL Server ODBC Driver | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.MSSQL.CMDLnUtils | SQL Server Command Line Utilities | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.PortableLibrary | .NET Portable Library targeting pack | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.DataSources | Data sources for SQL Server support | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.LocalDB.Runtime | SQL Server Express 2019 LocalDB | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.SSDT | SQL Server Data Tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Wcf.Tooling | Windows Communication Foundation | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.MSIX.Packaging | MSIX Packaging Tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.WindowsAppSDK.Cs | Windows App SDK C# Templates | 17.4.33006.217 | Optional

## Game development with Unity

**ID:** Microsoft.VisualStudio.Workload.ManagedGame

**Description:** Create 2D and 3D games with Unity, a powerful cross-platform development environment.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Net.Component.4.7.1.TargetingPack | .NET Framework 4.7.1 targeting pack | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Unity | Visual Studio Tools for Unity | 17.4.33006.217 | Required
Component.UnityEngine.x64 | Unity Hub | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended

## Linux and embedded development with C++

**ID:** Microsoft.VisualStudio.Workload.NativeCrossPlat

**Description:** Create and debug applications running in a Linux environment or on an embedded device.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Component.MDD.Linux | C++ for Linux Development | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Required
Component.CPython39.x64 | Python 3 64-bit (3.9.7) | 3.9.7 | Recommended
Component.Linux.CMake | C++ CMake tools for Linux | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Embedded | Embedded and IoT tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Recommended
Component.MDD.Linux.GCC.arm | Legacy Embedded and IoT tools | 17.4.33006.217 | Optional

## Desktop development with C++

**ID:** Microsoft.VisualStudio.Workload.NativeDesktop

**Description:** Build modern C++ apps for Windows using tools of your choice, including MSVC, Clang, CMake, or MSBuild.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.VC.Redist.14.Latest | C++ 2022 Redistributable Update | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.NativeDesktop.Core | C++ core desktop features | 17.4.33006.217 | Required
Component.Microsoft.VisualStudio.LiveShare.2022 | Live Share | 1.0.5716 | Recommended
Microsoft.VisualStudio.Component.Debugger.JustInTime | Just-In-Time debugger | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Graphics | Image and 3D model editors | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Graphics.Tools | Graphics debugger and GPU profiler for DirectX | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.ASAN | C++ AddressSanitizer | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.ATL | C++ ATL for latest v143 build tools (x86 & x64) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.ATL.ARM64 | C++ ATL for latest v143 build tools (ARM64) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.CMake.Project | C++ CMake tools for Windows | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.DiagnosticTools | C++ profiling tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.TestAdapterForBoostTest | Test Adapter for Boost.Test | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.TestAdapterForGoogleTest | Test Adapter for Google Test | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.Tools.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (Latest) | 17.4.33027.87 | Recommended
Microsoft.VisualStudio.Component.VC.Tools.ARM64EC | MSVC v143 - VS 2022 C++ ARM64EC build tools (Latest) | 17.4.33027.87 | Recommended
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Windows11SDK.22000 | Windows 11 SDK (10.0.22000.0) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Windows11SDK.22621 | Windows 11 SDK (10.0.22621.0) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions.CMake | JSON editor | 17.4.33006.217 | Recommended
Component.Incredibuild | Incredibuild - Build Acceleration | 17.4.33006.217 | Optional
Component.IncredibuildMenu | IncredibuildMenu | 1.6.0.4 | Optional
Microsoft.Component.VC.Runtime.UCRTSDK | Windows Universal CRT SDK | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.UWP.VC.ARM64 | C++ Universal Windows Platform support for v143 build tools (ARM64) | 17.4.33027.87 | Optional
Microsoft.VisualStudio.Component.UWP.VC.ARM64EC | C++ Universal Windows Platform support for v143 build tools (ARM64EC) | 17.4.33027.87 | Optional
Microsoft.VisualStudio.Component.VC.140 | MSVC v140 - VS 2015 C++ build tools (v14.00) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.ATLMFC | C++ MFC for latest v143 build tools (x86 & x64) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.CLI.Support | C++/CLI support for v143 build tools (Latest) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Llvm.Clang | C++ Clang Compiler for Windows (15.0.1) | 17.4.33015.44 | Optional
Microsoft.VisualStudio.Component.VC.Llvm.ClangToolset | C++ Clang-cl for v143 build tools (x64/x86) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.MFC.ARM64 | C++ MFC for latest v143 build tools (ARM64) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Modules.ARM64 | C++ Modules for v143 build tools (ARM64 – experimental) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Modules.x86.x64 | C++ Modules for v143 build tools (x64/x86 – experimental) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Tools.ARM | MSVC v143 - VS 2022 C++ ARM build tools (Latest) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.v141.x86.x64 | MSVC v141 - VS 2017 C++ x64/x86 build tools (v14.16) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.18362 | Windows 10 SDK (10.0.18362.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.19041 | Windows 10 SDK (10.0.19041.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.20348 | Windows 10 SDK (10.0.20348.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.NativeDesktop.Llvm.Clang | C++ Clang tools for Windows (15.0.1 - x64/x86) | 17.4.33015.44 | Optional
Microsoft.VisualStudio.ComponentGroup.UWP.VC | C++ (v143) Universal Windows Platform tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.VC.Tools.142.x86.x64 | MSVC v142 - VS 2019 C++ x64/x86 build tools (v14.29) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.WindowsAppSDK.Cpp | Windows App SDK C++ Templates | 17.4.33006.217 | Optional

## Game development with C++

**ID:** Microsoft.VisualStudio.Workload.NativeGame

**Description:** Use the full power of C++ to build professional games powered by DirectX, Unreal, or Cocos2d.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.VC.Redist.14.Latest | C++ 2022 Redistributable Update | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Windows10SDK | Windows Universal C Runtime | 17.4.33006.217 | Required
Component.Unreal.Ide | IDE support for Unreal Engine | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Graphics | Image and 3D model editors | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Graphics.Tools | Graphics debugger and GPU profiler for DirectX | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.VC.ASAN | C++ AddressSanitizer | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.DiagnosticTools | C++ profiling tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.VC.Tools.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (Latest) | 17.4.33027.87 | Recommended
Microsoft.VisualStudio.Component.VC.Tools.ARM64EC | MSVC v143 - VS 2022 C++ ARM64EC build tools (Latest) | 17.4.33027.87 | Recommended
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Windows11SDK.22000 | Windows 11 SDK (10.0.22000.0) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Windows11SDK.22621 | Windows 11 SDK (10.0.22621.0) | 17.4.33006.217 | Recommended
Component.Android.NDK.R23C | Android NDK (R23C) | 17.4.33006.217 | Optional
Component.Android.SDK.MAUI | Android SDK setup (API level 33) | 17.4.33006.217 | Optional
Component.Cocos | Cocos | 17.4.33006.217 | Optional
Component.Incredibuild | Incredibuild - Build Acceleration | 17.4.33006.217 | Optional
Component.IncredibuildMenu | IncredibuildMenu | 1.6.0.4 | Optional
Component.MDD.Android | C++ Android development tools | 17.4.33006.217 | Optional
Component.OpenJDK | OpenJDK (Microsoft distribution) | 17.4.33006.217 | Optional
Component.Unreal | Unreal Engine installer | 17.4.33006.217 | Optional
Component.Unreal.Android | Android IDE support for Unreal Engine | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.6.2.TargetingPack | .NET Framework 4.6.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.TargetingPack | .NET Framework 4.8 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.TargetingPacks.Common | .NET Framework 4.8 development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.NuGet.BuildTools | NuGet targets and build tasks | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.18362 | Windows 10 SDK (10.0.18362.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.19041 | Windows 10 SDK (10.0.19041.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.20348 | Windows 10 SDK (10.0.20348.0) | 17.4.33006.217 | Optional

## Mobile development with C++

**ID:** Microsoft.VisualStudio.Workload.NativeMobile

**Description:** Build cross-platform applications for iOS, Android or Windows using C++.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Component.Android.SDK.MAUI | Android SDK setup (API level 33) | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Required
Component.Android.Emulator.MDD | Google Android Emulator (local install) | 17.4.33006.217 | Recommended
Component.Android.NDK.R23C | Android NDK (R23C) | 17.4.33006.217 | Recommended
Component.HAXM.Private | Intel Hardware Accelerated Execution Manager (HAXM) (local install) | 17.4.33006.217 | Recommended
Component.MDD.Android | C++ Android development tools | 17.4.33006.217 | Recommended
Component.OpenJDK | OpenJDK (Microsoft distribution) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Component.Incredibuild | Incredibuild - Build Acceleration | 17.4.33006.217 | Optional
Component.IncredibuildMenu | IncredibuildMenu | 1.6.0.4 | Optional
Component.MDD.IOS | C++ iOS development tools | 17.4.33006.217 | Optional

## .NET Multi-platform App UI development

**ID:** Microsoft.VisualStudio.Workload.NetCrossPlat

**Description:** Build Android, iOS, Windows, and Mac apps from a single codebase using C# with .NET MAUI.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
android | .NET SDK for Android | 33.0.4.0 | Required
Component.Android.SDK.MAUI | Android SDK setup (API level 33) | 17.4.33006.217 | Required
Component.OpenJDK | OpenJDK (Microsoft distribution) | 17.4.33006.217 | Required
Component.Xamarin.RemotedSimulator | Xamarin Remoted Simulator | 17.4.33006.217 | Required
ios | .NET SDK for iOS | 16.0.527.1478 | Required
maccatalyst | .NET SDK for Mac Catalyst | 15.4.1186.2372 | Required
maui.android | .NET MAUI SDK for Android | 7.0.49.0 | Required
maui.blazor | .NET MAUI SDK for Blazor Desktop | 7.0.49.0 | Required
maui.core | .NET MAUI SDK Core | 7.0.49.0 | Required
maui.ios | .NET MAUI SDK for iOS | 7.0.49.0 | Required
maui.maccatalyst | .NET MAUI SDK for Mac Catalyst | 7.0.49.0 | Required
maui.windows | .NET MAUI SDK for Windows | 7.0.49.0 | Required
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.ComponentGroup.ClickOnce.Publish | ClickOnce Publishing for .NET  | 17.4.33015.44 | Required
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Required
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Required
microsoft.net.runtime.android | .NET Android Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.android.aot | .NET Android Build Tools (AoT) | 7.0.22.51805 | Required
microsoft.net.runtime.android.aot.net6 | .NET 6.0 Android Build Tools (AoT) | 7.0.22.51805 | Required
microsoft.net.runtime.android.net6 | .NET 6.0 Android Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.ios | .NET iOS Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.ios.net6 | .NET 6.0 iOS Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.maccatalyst | .NET Mac Catalyst Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.maccatalyst.net6 | .NET 6.0 Mac Catalyst Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.mono.tooling | .NET Shared Mobile Build Tools | 7.0.22.51805 | Required
microsoft.net.runtime.mono.tooling.net6 | .NET 6.0 Shared Mobile Build Tools | 7.0.22.51805 | Required
Microsoft.NetCore.Component.DevelopmentTools | Development tools for .NET | 17.4.33006.217 | Required
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Required
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Required
Microsoft.VisualStudio.Component.FSharp | F# language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Merq | Common Xamarin internal tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MonoDebugger | Mono debugger | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.All | .NET MAUI | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.Android | .NET MAUI for Android | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.Blazor | Blazor support for .NET MAUI Applications | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.iOS | .NET MAUI for iOS | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.MacCatalyst | .NET MAUI for Mac Catalyst | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.Shared | .NET MAUI development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Maui.Windows | .NET MAUI for Windows | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.MSIX.Packaging | MSIX Packaging Tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions.TemplateEngine | ASP.NET templating engine | 17.4.33006.217 | Required
runtimes.ios | .NET iOS Runtimes | 7.0.22.51805 | Required
runtimes.ios.net6 | .NET 6.0 iOS Runtimes | 7.0.22.51805 | Required
runtimes.maccatalyst | .NET Mac Catalyst Build Tools | 7.0.22.51805 | Required
runtimes.maccatalyst.net6 | .NET 6.0 Mac Catalyst Build Tools | 7.0.22.51805 | Required
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Component.Xamarin | Xamarin | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional

## ASP.NET and web development

**ID:** Microsoft.VisualStudio.Workload.NetWeb

**Description:** Build web applications using ASP.NET Core, ASP.NET, HTML/JavaScript, and Containers including Docker support.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Component.Microsoft.VisualStudio.RazorExtension | Razor Language Services | 17.4.33006.217 | Required
Component.Microsoft.Web.LibraryManager | Library Manager | 17.4.33006.217 | Required
Component.Microsoft.WebTools.BrowserLink.WebLivePreview | Web Live Preview | 17.4.51.37770 | Required
Microsoft.Component.ClickOnce | ClickOnce Publishing | 17.4.33006.217 | Required
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.ComponentGroup.ClickOnce.Publish | ClickOnce Publishing for .NET  | 17.4.33015.44 | Required
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Required
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Required
Microsoft.NetCore.Component.DevelopmentTools | Development tools for .NET | 17.4.33006.217 | Required
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Required
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Web | Web development tools for .NET | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.DockerTools | Container development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.FSharp | F# language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.FSharp.WebTemplates | F# language support for web projects | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.IISExpress | IIS Express  | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.ManagedDesktop.Core | Managed Desktop Workload Core | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MSODBC.SQL | SQL Server ODBC Driver | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MSSQL.CMDLnUtils | SQL Server Command Line Utilities | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.DataSources | Data sources for SQL Server support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.LocalDB.Runtime | SQL Server Express 2019 LocalDB | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.SSDT | SQL Server Data Tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Required
Component.Microsoft.VisualStudio.LiveShare.2022 | Live Share | 1.0.5716 | Recommended
Component.Microsoft.VisualStudio.Web.AzureFunctions | Azure WebJobs Tools | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.1.SDK | .NET Framework 4.8.1 SDK | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.1.TargetingPack | .NET Framework 4.8.1 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.8.TargetingPack | .NET Framework 4.8 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.4.8.1.DeveloperTools | .NET Framework 4.8.1 development tools | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.4.8.DeveloperTools | .NET Framework 4.8 development tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Debugger.JustInTime | Just-In-Time debugger | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.DiagnosticTools | .NET profiling tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.EntityFramework | Entity Framework 6 tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.WslDebugging | .NET Debugging with WSL | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.AzureFunctions | Azure WebJobs Tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.ComponentGroup.Web.CloudTools | Cloud tools for web development | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.6.2.TargetingPack | .NET Framework 4.6.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.1.TargetingPack | .NET Framework 4.7.1 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.TargetingPack | .NET Framework 4.7 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.4.6.2-4.7.1.DeveloperTools | .NET Framework 4.6.2-4.7.1 development tools | 17.4.33006.217 | Optional
microsoft.net.runtime.mono.tooling | .NET Shared Mobile Build Tools | 7.0.22.51805 | Optional
microsoft.net.runtime.mono.tooling.net6 | .NET 6.0 Shared Mobile Build Tools | 7.0.22.51805 | Optional
microsoft.net.sdk.emscripten.net6 | Emscripten SDK compiler tooling | 7.0.7.1101 | Optional
microsoft.net.sdk.emscripten.net7 | Emscripten SDK compiler tooling | 7.0.7.1101 | Optional
Microsoft.VisualStudio.Component.AspNet | .NET Framework project and item templates | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.AspNet45 | Advanced ASP.NET features | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TeamsFx | Microsoft Teams development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Wcf.Tooling | Windows Communication Foundation | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.AdditionalWebProjectTemplates | Additional project templates (previous versions) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.IISDevelopment | Development time IIS support | 17.4.33006.217 | Optional
wasm.tools | .NET WebAssembly Build Tools | 7.0.22.51805 | Optional
wasm.tools.net6 | .NET 6.0 WebAssembly Build Tools | 7.0.22.51805 | Optional

## Node.js development

**ID:** Microsoft.VisualStudio.Workload.Node

**Description:** Build scalable network applications using Node.js, an asynchronous event-driven JavaScript runtime. 

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Node.Tools | Node.js development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Required
Component.Microsoft.VisualStudio.LiveShare.2022 | Live Share | 1.0.5716 | Recommended
Microsoft.VisualStudio.Component.Debugger.JustInTime | Just-In-Time debugger | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest) | 17.4.33006.217 | Optional

## Office/SharePoint development

**ID:** Microsoft.VisualStudio.Workload.Office

**Description:** Create Office and SharePoint add-ins, SharePoint solutions, and VSTO add-ins using C#, VB, and JavaScript.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Component.Microsoft.VisualStudio.RazorExtension | Razor Language Services | 17.4.33006.217 | Required
Component.Microsoft.Web.LibraryManager | Library Manager | 17.4.33006.217 | Required
Component.Microsoft.WebTools.BrowserLink.WebLivePreview | Web Live Preview | 17.4.51.37770 | Required
Microsoft.Component.ClickOnce | ClickOnce Publishing | 17.4.33006.217 | Required
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.ComponentGroup.ClickOnce.Publish | ClickOnce Publishing for .NET  | 17.4.33015.44 | Required
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Required
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Required
Microsoft.NetCore.Component.DevelopmentTools | Development tools for .NET | 17.4.33006.217 | Required
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Required
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Web | Web development tools for .NET | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.DockerTools | Container development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.FSharp | F# language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.FSharp.WebTemplates | F# language support for web projects | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.IISExpress | IIS Express  | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.ManagedDesktop.Core | Managed Desktop Workload Core | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.ManagedDesktop.Prerequisites | .NET desktop development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MSODBC.SQL | SQL Server ODBC Driver | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.MSSQL.CMDLnUtils | SQL Server Command Line Utilities | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Sharepoint.Tools | Office Developer Tools for Visual Studio | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.DataSources | Data sources for SQL Server support | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.LocalDB.Runtime | SQL Server Express 2019 LocalDB | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.SSDT | SQL Server Data Tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Wcf.Tooling | Windows Communication Foundation | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Workflow | Windows Workflow Foundation | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.TargetingPack | .NET Framework 4.8 targeting pack | 17.4.33006.217 | Recommended
Microsoft.Net.ComponentGroup.4.8.DeveloperTools | .NET Framework 4.8 development tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.TeamOffice | Visual Studio Tools for Office (VSTO) | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Recommended
Microsoft.Net.Component.4.6.2.TargetingPack | .NET Framework 4.6.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.1.TargetingPack | .NET Framework 4.7.1 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.TargetingPack | .NET Framework 4.7 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.1.SDK | .NET Framework 4.8.1 SDK | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.1.TargetingPack | .NET Framework 4.8.1 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.4.6.2-4.7.1.DeveloperTools | .NET Framework 4.6.2-4.7.1 development tools | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.4.8.1.DeveloperTools | .NET Framework 4.8.1 development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.Sharepoint.WIF | Windows Identity Foundation 3.5 | 17.4.33006.217 | Optional

## Python development

**ID:** Microsoft.VisualStudio.Workload.Python

**Description:** Editing, debugging, interactive development and source control for Python.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.PythonTools | Python language support | 17.4.33006.217 | Required
Component.CPython39.x64 | Python 3 64-bit (3.9.7) | 3.9.7 | Optional
Component.Microsoft.VisualStudio.LiveShare.2022 | Live Share | 1.0.5716 | Optional
Component.Microsoft.VisualStudio.RazorExtension | Razor Language Services | 17.4.33006.217 | Optional
Component.Microsoft.Web.LibraryManager | Library Manager | 17.4.33006.217 | Optional
Component.Microsoft.WebTools.BrowserLink.WebLivePreview | Web Live Preview | 17.4.51.37770 | Optional
Microsoft.Component.ClickOnce | ClickOnce Publishing | 17.4.33006.217 | Optional
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Optional
Microsoft.Component.PythonTools.Web | Python web support | 17.4.33006.217 | Optional
Microsoft.ComponentGroup.ClickOnce.Publish | ClickOnce Publishing for .NET  | 17.4.33015.44 | Optional
Microsoft.ComponentGroup.PythonTools.NativeDevelopment | Python native development tools | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Optional
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Optional
Microsoft.NetCore.Component.DevelopmentTools | Development tools for .NET | 17.4.33006.217 | Optional
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Optional
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Optional
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Optional
Microsoft.NetCore.Component.Web | Web development tools for .NET | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Azure.AuthoringTools | Azure Authoring Tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Azure.ClientLibs | Azure libraries for .NET | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Azure.Compute.Emulator | Azure Compute Emulator | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Azure.Waverton | Azure Cloud Services core tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Azure.Waverton.BuildTools | Azure Cloud Services build tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Common.Azure.Tools | Connectivity and publishing tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Debugger.JustInTime | Just-In-Time debugger | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.DockerTools | Container development tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.FSharp | F# language support | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.FSharp.WebTemplates | F# language support for web projects | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Graphics.Tools | Graphics debugger and GPU profiler for DirectX | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.IISExpress | IIS Express  | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.JavaScript.Diagnostics | JavaScript diagnostics | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.JavaScript.TypeScript | JavaScript and TypeScript language support | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.ManagedDesktop.Core | Managed Desktop Workload Core | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.MSODBC.SQL | SQL Server ODBC Driver | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.MSSQL.CMDLnUtils | SQL Server Command Line Utilities | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.DataSources | Data sources for SQL Server support | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.LocalDB.Runtime | SQL Server Express 2019 LocalDB | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.SQL.SSDT | SQL Server Data Tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.SDK.4.8 | TypeScript 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.TypeScript.TSServer | TypeScript Server | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.DiagnosticTools | C++ profiling tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.WebDeploy | Web Deploy | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK | Windows Universal C Runtime | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows11SDK.22000 | Windows 11 SDK (10.0.22000.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.Web | ASP.NET and web development prerequisites | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.WebToolsExtensions | ASP.NET and web development | 17.4.33006.217 | Optional

## Universal Windows Platform development

**ID:** Microsoft.VisualStudio.Workload.Universal

**Description:** Create applications for the Universal Windows Platform with C#, VB, or optionally C﻿+﻿+.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.NetFX.Native | .NET Native | 17.4.33006.217 | Required
Microsoft.ComponentGroup.Blend | Blend for Visual Studio | 17.4.33006.217 | Required
Microsoft.NetCore.Component.Runtime.6.0 | .NET 6.0 Runtime (Long Term Support) | 17.4.33103.184 | Required
Microsoft.NetCore.Component.Runtime.7.0 | .NET 7.0 Runtime | 17.4.33103.184 | Required
Microsoft.NetCore.Component.SDK | .NET SDK | 17.4.33103.184 | Required
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.DiagnosticTools | .NET profiling tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Graphics | Image and 3D model editors | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.SQL.CLR | CLR data types for SQL Server | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Windows11SDK.22000 | Windows 11 SDK (10.0.22000.0) | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Windows11SDK.22621 | Windows 11 SDK (10.0.22621.0) | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.MSIX.Packaging | MSIX Packaging Tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.UWP.NetCoreAndStandard | .NET Native and .NET Standard | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.UWP.Support | Universal Windows Platform tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.UWP.Xamarin | Universal Windows Platform tools for Xamarin | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Graphics.Tools | Graphics debugger and GPU profiler for DirectX | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.UWP.VC.ARM64 | C++ Universal Windows Platform support for v143 build tools (ARM64) | 17.4.33027.87 | Optional
Microsoft.VisualStudio.Component.UWP.VC.ARM64EC | C++ Universal Windows Platform support for v143 build tools (ARM64EC) | 17.4.33027.87 | Optional
Microsoft.VisualStudio.Component.VC.14.29.16.11.ARM | MSVC v142 - VS 2019 C++ ARM build tools (v14.29-16.11) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.14.29.16.11.ARM64 | MSVC v142 - VS 2019 C++ ARM64 build tools (v14.29-16.11) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.CoreIde | C++ core features | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Tools.ARM | MSVC v143 - VS 2022 C++ ARM build tools (Latest) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.Tools.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (Latest) | 17.4.33027.87 | Optional
Microsoft.VisualStudio.Component.VC.Tools.ARM64EC | MSVC v143 - VS 2022 C++ ARM64EC build tools (Latest) | 17.4.33027.87 | Optional
Microsoft.VisualStudio.Component.VC.Tools.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (Latest) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.v141.ARM | MSVC v141 - VS 2017 C++ ARM build tools (v14.16) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.v141.ARM64 | MSVC v141 - VS 2017 C++ ARM64 build tools (v14.16) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.VC.v141.x86.x64 | MSVC v141 - VS 2017 C++ x64/x86 build tools (v14.16) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.18362 | Windows 10 SDK (10.0.18362.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.19041 | Windows 10 SDK (10.0.19041.0) | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.Windows10SDK.IpOverUsb | USB Device Connectivity | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.UWP.VC | C++ (v143) Universal Windows Platform tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.UWP.VC.v141 | C++ (v141) Universal Windows Platform tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.UWP.VC.v142 | C++ (v142) Universal Windows Platform tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.ComponentGroup.VC.Tools.142.x86.x64 | MSVC v142 - VS 2019 C++ x64/x86 build tools (v14.29) | 17.4.33006.217 | Optional

## Visual Studio extension development

**ID:** Microsoft.VisualStudio.Workload.VisualStudioExtension

**Description:** Create add-ons and extensions for Visual Studio, including new commands, code analyzers and tool windows.

### Components included by this workload

Component ID | Name | Version | Dependency type
--- | --- | --- | ---
Microsoft.Component.MSBuild | MSBuild | 17.4.33006.217 | Required
Microsoft.Net.Component.4.6.TargetingPack | .NET Framework 4.6 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.7.2.TargetingPack | .NET Framework 4.7.2 targeting pack | 17.4.33006.217 | Required
Microsoft.Net.Component.4.8.SDK | .NET Framework 4.8 SDK | 17.4.33006.217 | Required
Microsoft.Net.ComponentGroup.DevelopmentPrerequisites | .NET Framework 4.7.2 development tools | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.NuGet | NuGet package manager | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.Compiler | C# and Visual Basic Roslyn compilers | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.Roslyn.LanguageServices | C# and Visual Basic | 17.4.33006.217 | Required
Microsoft.VisualStudio.Component.VSSDK | Visual Studio SDK | 17.4.33006.217 | Required
Microsoft.VisualStudio.ComponentGroup.VisualStudioExtension.Prerequisites | Visual Studio extension development prerequisites | 17.4.33006.217 | Required
Microsoft.Component.CodeAnalysis.SDK | .NET Compiler Platform SDK | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.DiagnosticTools | .NET profiling tools | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.IntelliCode | IntelliCode | 17.4.33027.239 | Recommended
Microsoft.VisualStudio.Component.TextTemplating | Text Template Transformation | 17.4.33006.217 | Recommended
Microsoft.VisualStudio.Component.AppInsights.Tools | Developer Analytics tools | 17.4.33006.217 | Optional
Microsoft.VisualStudio.Component.DslTools | Modeling SDK | 17.4.33006.217 | Optional

## Unaffiliated components

These are components that are not included with any workload, but may be selected as an individual component.

Component ID | Name | Version
--- | --- | ---
Microsoft.Component.HelpViewer | Help Viewer | 17.4.33006.217
Microsoft.Net.Component.3.5.DeveloperTools | .NET Framework 3.5 development tools | 17.4.33006.217
Microsoft.Net.Component.3.5.DeveloperTools | .NET Framework 3.5 development tools | 17.4.33006.217
Microsoft.Net.Component.4.6.1.SDK | .NET Framework 4.6.1 SDK | 17.4.33006.217
Microsoft.Net.Component.4.6.1.SDK | .NET Framework 4.6.1 SDK | 17.4.33006.217
Microsoft.Net.Component.4.6.2.SDK | .NET Framework 4.6.2 SDK | 17.4.33006.217
Microsoft.Net.Component.4.6.2.SDK | .NET Framework 4.6.2 SDK | 17.4.33006.217
Microsoft.Net.Component.4.7.1.SDK | .NET Framework 4.7.1 SDK | 17.4.33006.217
Microsoft.Net.Component.4.7.1.SDK | .NET Framework 4.7.1 SDK | 17.4.33006.217
Microsoft.Net.Component.4.7.2.SDK | .NET Framework 4.7.2 SDK | 17.4.33006.217
Microsoft.Net.Component.4.7.2.SDK | .NET Framework 4.7.2 SDK | 17.4.33006.217
Microsoft.Net.Component.4.7.SDK | .NET Framework 4.7 SDK | 17.4.33006.217
Microsoft.Net.Component.4.7.SDK | .NET Framework 4.7 SDK | 17.4.33006.217
Microsoft.Net.Core.Component.SDK.2.1 | .NET Core 2.1 Runtime (Out of support) | 17.4.33103.184
Microsoft.NetCore.Component.Runtime.3.1 | .NET Core 3.1 Runtime (Long Term Support) | 17.4.33103.184
Microsoft.NetCore.Component.Runtime.5.0 | .NET 5.0 Runtime (Out of support) | 17.4.33103.184
Microsoft.NetCore.ComponentGroup.DevelopmentTools.2.1 | Development Tools for .NET Core 2.1 (Out of support) | 17.4.33103.184
Microsoft.NetCore.ComponentGroup.Web.2.1 | Web development tools for .NET Core 2.1 (Out of support) | 17.4.33103.184
Microsoft.VisualStudio.Component.AzureDevOps.OfficeIntegration | Azure DevOps Office Integration | 17.4.33006.217
Microsoft.VisualStudio.Component.ClassDesigner | Class Designer | 17.4.33006.217
Microsoft.VisualStudio.Component.DependencyValidation.Community | Dependency Validation | 17.4.33006.217
Microsoft.VisualStudio.Component.DependencyValidation.Community | Dependency Validation | 17.4.33006.217
Microsoft.VisualStudio.Component.Git | Git for Windows | 17.4.33006.217
Microsoft.VisualStudio.Component.Git | Git for Windows | 17.4.33006.217
Microsoft.VisualStudio.Component.GraphDocument | DGML editor | 17.4.33006.217
Microsoft.VisualStudio.Component.GraphDocument | DGML editor | 17.4.33006.217
Microsoft.VisualStudio.Component.LinqToSql | LINQ to SQL tools | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ARM.Spectre | MSVC v142 - VS 2019 C++ ARM Spectre-mitigated libs (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ARM.Spectre | MSVC v142 - VS 2019 C++ ARM Spectre-mitigated libs (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ARM64.Spectre | MSVC v142 - VS 2019 C++ ARM64 Spectre-mitigated libs (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ARM64.Spectre | MSVC v142 - VS 2019 C++ ARM64 Spectre-mitigated libs (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL | C++ v14.29 (16.11) ATL for v142 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL | C++ v14.29 (16.11) ATL for v142 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM | C++ v14.29 (16.11) ATL for v142 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM | C++ v14.29 (16.11) ATL for v142 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM.Spectre | C++ v14.29 (16.11) ATL for v142 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM.Spectre | C++ v14.29 (16.11) ATL for v142 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM64 | C++ v14.29 (16.11) ATL for v142 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM64 | C++ v14.29 (16.11) ATL for v142 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM64.Spectre | C++ v14.29 (16.11) ATL for v142 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.ARM64.Spectre | C++ v14.29 (16.11) ATL for v142 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.Spectre | C++ v14.29 (16.11) ATL for v142 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.ATL.Spectre | C++ v14.29 (16.11) ATL for v142 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.CLI.Support | C++/CLI support for v142 build tools (14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.CLI.Support | C++/CLI support for v142 build tools (14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC | C++ v14.29 (16.11) MFC for v142 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC | C++ v14.29 (16.11) MFC for v142 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM | C++ v14.29 (16.11) MFC for v142 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM | C++ v14.29 (16.11) MFC for v142 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM.Spectre | C++ v14.29 (16.11) MFC for v142 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM.Spectre | C++ v14.29 (16.11) MFC for v142 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM64 | C++ v14.29 (16.11) MFC for v142 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM64 | C++ v14.29 (16.11) MFC for v142 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM64.Spectre | C++ v14.29 (16.11) MFC for v142 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.ARM64.Spectre | C++ v14.29 (16.11) MFC for v142 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.Spectre | C++ v14.29 (16.11) MFC for v142 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.MFC.Spectre | C++ v14.29 (16.11) MFC for v142 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.x86.x64 | MSVC v142 - VS 2019 C++ x64/x86 build tools (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.x86.x64 | MSVC v142 - VS 2019 C++ x64/x86 build tools (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.x86.x64.Spectre | MSVC v142 - VS 2019 C++ x64/x86 Spectre-mitigated libs (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.29.16.11.x86.x64.Spectre | MSVC v142 - VS 2019 C++ x64/x86 Spectre-mitigated libs (v14.29-16.11) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ATL | C++ v14.30 (17.0) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ATL.ARM | C++ v14.30 (17.0) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ATL.ARM.Spectre | C++ v14.30 (17.0) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ATL.ARM64 | C++ v14.30 (17.0) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ATL.ARM64.Spectre | C++ v14.30 (17.0) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.ATL.Spectre | C++ v14.30 (17.0) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.CLI.Support | C++/CLI support for v143 build tools (14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.MFC | C++ v14.30 (17.0) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.MFC.ARM | C++ v14.30 (17.0) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.MFC.ARM.Spectre | C++ v14.30 (17.0) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.MFC.ARM64 | C++ v14.30 (17.0) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.MFC.ARM64.Spectre | C++ v14.30 (17.0) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.MFC.Spectre | C++ v14.30 (17.0) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.30.17.0.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.30-17.0) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ATL | C++ v14.31 (17.1) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ATL.ARM | C++ v14.31 (17.1) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ATL.ARM.Spectre | C++ v14.31 (17.1) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ATL.ARM64 | C++ v14.31 (17.1) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ATL.ARM64.Spectre | C++ v14.31 (17.1) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.ATL.Spectre | C++ v14.31 (17.1) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.CLI.Support | C++/CLI support for v143 build tools (14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.MFC | C++ v14.31 (17.1) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.MFC.ARM | C++ v14.31 (17.1) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.MFC.ARM.Spectre | C++ v14.31 (17.1) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.MFC.ARM64 | C++ v14.31 (17.1) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.MFC.ARM64.Spectre | C++ v14.31 (17.1) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.MFC.Spectre | C++ v14.31 (17.1) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.31.17.1.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.31-17.1) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ATL | C++ v14.32 (17.2) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ATL.ARM | C++ v14.32 (17.2) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ATL.ARM.Spectre | C++ v14.32 (17.2) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ATL.ARM64 | C++ v14.32 (17.2) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ATL.ARM64.Spectre | C++ v14.32 (17.2) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.ATL.Spectre | C++ v14.32 (17.2) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.CLI.Support | C++/CLI support for v143 build tools (14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.MFC | C++ v14.32 (17.2) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.MFC.ARM | C++ v14.32 (17.2) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.MFC.ARM.Spectre | C++ v14.32 (17.2) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.MFC.ARM64 | C++ v14.32 (17.2) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.MFC.ARM64.Spectre | C++ v14.32 (17.2) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.MFC.Spectre | C++ v14.32 (17.2) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.32.17.2.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.32-17.2) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL | C++ v14.33 (17.3) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL | C++ v14.33 (17.3) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM | C++ v14.33 (17.3) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM | C++ v14.33 (17.3) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM.Spectre | C++ v14.33 (17.3) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM.Spectre | C++ v14.33 (17.3) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM64 | C++ v14.33 (17.3) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM64 | C++ v14.33 (17.3) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM64.Spectre | C++ v14.33 (17.3) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.ARM64.Spectre | C++ v14.33 (17.3) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.Spectre | C++ v14.33 (17.3) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.ATL.Spectre | C++ v14.33 (17.3) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.CLI.Support | C++/CLI support for v143 build tools (14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.CLI.Support | C++/CLI support for v143 build tools (14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC | C++ v14.33 (17.3) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC | C++ v14.33 (17.3) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM | C++ v14.33 (17.3) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM | C++ v14.33 (17.3) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM.Spectre | C++ v14.33 (17.3) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM.Spectre | C++ v14.33 (17.3) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM64 | C++ v14.33 (17.3) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM64 | C++ v14.33 (17.3) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM64.Spectre | C++ v14.33 (17.3) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.ARM64.Spectre | C++ v14.33 (17.3) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.Spectre | C++ v14.33 (17.3) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.MFC.Spectre | C++ v14.33 (17.3) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.33.17.3.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.33-17.3) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM | MSVC v143 - VS 2022 C++ ARM build tools (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.34-17.4) | 17.4.33027.87
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM64 | MSVC v143 - VS 2022 C++ ARM64 build tools (v14.34-17.4) | 17.4.33027.87
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.34-17.4) | 17.4.33027.87
Microsoft.VisualStudio.Component.VC.14.34.17.4.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (v14.34-17.4) | 17.4.33027.87
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL | C++ v14.34 (17.4) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL | C++ v14.34 (17.4) ATL for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM | C++ v14.34 (17.4) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM | C++ v14.34 (17.4) ATL for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM.Spectre | C++ v14.34 (17.4) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM.Spectre | C++ v14.34 (17.4) ATL for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM64 | C++ v14.34 (17.4) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM64 | C++ v14.34 (17.4) ATL for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM64.Spectre | C++ v14.34 (17.4) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.ARM64.Spectre | C++ v14.34 (17.4) ATL for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.Spectre | C++ v14.34 (17.4) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.ATL.Spectre | C++ v14.34 (17.4) ATL for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.CLI.Support | C++/CLI support for v143 build tools (14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.CLI.Support | C++/CLI support for v143 build tools (14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC | C++ v14.34 (17.4) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC | C++ v14.34 (17.4) MFC for v143 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM | C++ v14.34 (17.4) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM | C++ v14.34 (17.4) MFC for v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM.Spectre | C++ v14.34 (17.4) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM.Spectre | C++ v14.34 (17.4) MFC for v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM64 | C++ v14.34 (17.4) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM64 | C++ v14.34 (17.4) MFC for v143 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM64.Spectre | C++ v14.34 (17.4) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.ARM64.Spectre | C++ v14.34 (17.4) MFC for v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.Spectre | C++ v14.34 (17.4) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.MFC.Spectre | C++ v14.34 (17.4) MFC for v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.x86.x64 | MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.14.34.17.4.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (v14.34-17.4) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.ARM | C++ ATL for latest v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.ARM | C++ ATL for latest v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.ARM.Spectre | C++ ATL for latest v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.ARM.Spectre | C++ ATL for latest v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.ARM64.Spectre | C++ ATL for latest v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.ARM64.Spectre | C++ ATL for latest v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.Spectre | C++ ATL for latest v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATL.Spectre | C++ ATL for latest v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATLMFC.Spectre | C++ MFC for latest v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.ATLMFC.Spectre | C++ MFC for latest v143 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.MFC.ARM | C++ MFC for latest v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.MFC.ARM | C++ MFC for latest v143 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.MFC.ARM.Spectre | C++ MFC for latest v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.MFC.ARM.Spectre | C++ MFC for latest v143 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.MFC.ARM64.Spectre | C++ MFC for latest v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.MFC.ARM64.Spectre | C++ MFC for latest v143 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.Redist.MSM | C++ 2022 Redistributable MSMs | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.Redist.MSM | C++ 2022 Redistributable MSMs | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.Runtimes.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (Latest) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.Runtimes.ARM.Spectre | MSVC v143 - VS 2022 C++ ARM Spectre-mitigated libs (Latest) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.Runtimes.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (Latest) | 17.4.33027.87
Microsoft.VisualStudio.Component.VC.Runtimes.ARM64.Spectre | MSVC v143 - VS 2022 C++ ARM64 Spectre-mitigated libs (Latest) | 17.4.33027.87
Microsoft.VisualStudio.Component.VC.Runtimes.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (Latest)  | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.Runtimes.x86.x64.Spectre | MSVC v143 - VS 2022 C++ x64/x86 Spectre-mitigated libs (Latest)  | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ARM.Spectre | MSVC v141 - VS 2017 C++ ARM Spectre-mitigated libs (v14.16) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ARM64.Spectre | MSVC v141 - VS 2017 C++ ARM64 Spectre-mitigated libs (v14.16) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ATL | C++ ATL for v141 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ATL.ARM | C++ ATL for v141 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ATL.ARM.Spectre | C++ ATL for v141 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ATL.ARM64 | C++ ATL for v141 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ATL.ARM64.Spectre | C++ ATL for v141 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.ATL.Spectre | C++ ATL for v141 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.CLI.Support | C++/CLI support for v141 build tools (14.16) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.MFC | C++ MFC for v141 build tools (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.MFC.ARM | C++ MFC for v141 build tools (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.MFC.ARM.Spectre | C++ MFC for v141 build tools with Spectre Mitigations (ARM) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.MFC.ARM64 | C++ MFC for v141 build tools (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.MFC.ARM64.Spectre | C++ MFC for v141 build tools with Spectre Mitigations (ARM64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.MFC.Spectre | C++ MFC for v141 build tools with Spectre Mitigations (x86 & x64) | 17.4.33006.217
Microsoft.VisualStudio.Component.VC.v141.x86.x64.Spectre | MSVC v141 - VS 2017 C++ x64/x86 Spectre-mitigated libs (v14.16) | 17.4.33006.217
Microsoft.VisualStudio.Component.VisualStudioData | Data sources and service references | 17.4.33006.217
Microsoft.VisualStudio.Component.WinXP | C++ Windows XP Support for VS 2017 (v141) tools [Deprecated] | 17.4.33006.217
Microsoft.VisualStudio.Web.Mvc4.ComponentGroup | ASP.NET MVC 4 | 17.4.33006.217
