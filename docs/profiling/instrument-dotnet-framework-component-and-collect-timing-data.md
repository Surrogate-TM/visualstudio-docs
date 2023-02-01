---
title: Profiler command line - Instrument client .NET component, get time data
description: Learn how to use the Visual Studio Profiling Tools command-line tools to collect timing data for a .NET Framework component of a stand-alone application.
ms.date: 11/11/2022
ms.topic: how-to
ms.assetid: b7dcc27b-45c6-4302-9552-6fa5b1e94b56
author: mikejo5000
ms.author: mikejo
manager: jmartens
ms.technology: vs-ide-debug
ms.workload: 
  - dotnet
---
# How to: Instrument a stand-alone .NET Framework component and collect timing data with the profiler from the command line

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]

This topic describes how to use Visual Studio command-line profiling tools to instrument a .NET Framework, .NET Core, or .NET 5+ component such as an .*exe* or .*dll* file, and to collect detailed timing data.

> [!NOTE]
> To get the path to the profiling tools, see [Specify the path to command line tools](/previous-versions/visualstudio/visual-studio-2017/profiling/specifying-the-path-to-profiling-tools-command-line-tools). On 64-bit computers, both 64-bit and 32-bit versions of the tools are available. To use the profiler command-line tools, you must add the tools path to the PATH environment variable of the Command Prompt window or add it to the command itself.

 To collect detailed timing data from a .NET Framework component by using the instrumentation method, you use the [VSInstr.exe](../profiling/vsinstr.md) tool to generate an instrumented version of the component and the [VSPerfCLREnv.cmd](../profiling/vsperfclrenv.md) tool to initialize profiling environment variables. You then start the profiler.

 When the instrumented component is executed, timing data is automatically collected to a data file. You can pause and resume data collection during the profiling session.

 To end a profiling session, you close the target application and explicitly shut down the profiler. In most cases, we recommend clearing the profiling environment variables at the end of a session.

## Start the profiling session

To start profiling by using the instrumentation method:

1. Open a Command Prompt window. If necessary, add the profiler tools directory to your PATH environment variable. The path is not added at installation.

2. Use the **VSInstr** tool to generate an instrumented version of the target application.

3. Initialize the .NET Framework profiling environment variables. Type:

    **VSPerfClrEnv /traceon**

4. Start the profiler. Type:

    **VSPerfCmd /start:trace /output:** `OutputFile` [`Options`]

   - The [/start](/previous-versions/visualstudio/visual-studio-2017/profiling/start)**:trace** option initializes the profiler.

   - The [/output](/previous-versions/visualstudio/visual-studio-2017/profiling/output)**:**`OutputFile` option is required with **/start**. `OutputFile` specifies the name and location of the profiling data (.vsp) file.

     You can use any one of the following options with the **/start:trace** option.

   | Option | Description |
   | - | - |
   | [/user](/previous-versions/visualstudio/visual-studio-2017/profiling/user-vsperfcmd) **:**[`Domain`**\\**]`UserName` | Specifies the domain and user name of the account that owns the profiled process. This option is required only if the process is running as a user other than the logged-on user. The process owner is listed in the **User Name** column on the **Processes** tab of Windows Task Manager. |
   | [/crosssession](/previous-versions/visualstudio/visual-studio-2017/profiling/crosssession) | Enables profiling of processes in other sessions. This option is required if the ASP.NET application is running in a different session. The session identifier is listed in the **Session ID** column on the **Processes** tab of Windows Task Manager. **/CS** can be specified as an abbreviation for **/crosssession**. |
   | [/globaloff](/previous-versions/visualstudio/visual-studio-2017/profiling/globalon-and-globaloff) | Starts the profiler with data collection paused. Use [/globalon](../profiling/globalon-and-globaloff.md) to resume profiling. |
   | [/counter](/previous-versions/visualstudio/visual-studio-2017/profiling/counter) **:** `Config` | Collects information from the processor performance counter that is specified in `Config`. Counter information is added to the data that is collected at each profiling event. |
   | [/wincounter](/previous-versions/visualstudio/visual-studio-2017/profiling/wincounter) **:** `WinCounterPath` | Specifies a Windows performance counter to be collected during profiling. |
   | [/automark](/previous-versions/visualstudio/visual-studio-2017/profiling/automark) **:** `Interval` | Use with **/wincounter** only. Specifies the number of milliseconds between Windows performance counter collection events. Default is 500 ms. |
   | [/events](/previous-versions/visualstudio/visual-studio-2017/profiling/events-vsperfcmd) **:** `Config` | Specifies an Event Tracing for Windows (ETW) event to be collected during profiling. ETW events are collected in a separate (.*etl*) file. |

5. Start the target application from the Command Prompt window.

## Control data collection

When the target application is running, you can control data collection by starting and stopping the writing of data to the profiler data file by using *VSPerfCmd.exe* options. Controlling data collection enables you to collect data for a specific part of program execution, such as starting or shutting down the application.

To start and stop data collection:

- The following pairs of options start and stop data collection. Specify each option on a separate command line. You can turn data collection on and off multiple times.

    |Option|Description|
    |------------|-----------------|
    |[/globalon /globaloff](/previous-versions/visualstudio/visual-studio-2017/profiling/globalon-and-globaloff)|Starts (**/globalon**) or stops (**/globaloff**) data collection for all processes.|
    |[/processon](/previous-versions/visualstudio/visual-studio-2017/profiling/processon-and-processoff) **:** `PID` [/processoff](/previous-versions/visualstudio/visual-studio-2017/profiling/processon-and-processoff) **:** `PID`|Starts (**/processon**) or stops (**/processoff**) data collection for the process specified by the process ID (`PID`).|
    |[/threadon](/previous-versions/visualstudio/visual-studio-2017/profiling/threadon-and-threadoff) **:** `TID` [/threadoff](/previous-versions/visualstudio/visual-studio-2017/profiling/threadon-and-threadoff) **:** `TID`|Starts (**/threadon**) or stops (**/threadoff**) data collection for the thread specified by the thread ID (`TID`).|

## End the profiling session

 To end a profiling session, close the application that is running the instrumented component. Call the **VSPerfCmd** [/shutdown](/previous-versions/visualstudio/visual-studio-2017/profiling/shutdown) option to turn off the profiler and close the profiling data file. The **VSPerfClrEnv /off** command clears the profiling environment variables.

To end a profiling session:

1. Close the target application.

2. Shut down the profiler. Type:

     **VSPerfCmd /shutdown**

3. (Optional) Clear the profiling environment variables. Type:

     **VSPerfClrEnv /off**

## Reference

- [VSIntr](../profiling/vsinstr.md)
- [VSPerfCmd](../profiling/vsperfcmd.md)
