---
title: 'Command-line shells & prompt for developers'
description:  Start from the Tools > Command Line menu. Select the Visual Studio Developer Command Prompt, Developer PowerShell, or terminal to use .NET and C++ tools more easily.
author: TerryGLee
ms.author: tglee
ms.date: 01/23/2023
ms.topic: conceptual
ms.custom: contperf-fy21q4
helpviewer_keywords:
  - "Visual Studio command prompt"
  - "command prompt, Visual Studio"
  - "Developer Command Prompt"
  - "Developer PowerShell"
  - "Visual Studio terminal"
ms.assetid: 94fcf524-9045-4993-bfb2-e2d8bad44219
no-loc: cmdlet
monikerRange: ">=vs-2019"
---
# Visual Studio Developer Command Prompt and Developer PowerShell

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]

Visual Studio includes two command-line shells for developers, a command prompt and an instance of PowerShell, as follows:

- **Visual Studio Developer Command Prompt** - A standard command prompt with certain environment variables set to make using command-line developer tools easier. Available since Visual Studio 2015.

    ::: moniker range="vs-2019"
    :::image type="content" source="media/developer-command-prompt-for-vs/command-prompt.png" alt-text="Screenshot of the Developer Command Prompt for Visual Studio 2019 showing clrver tool.":::
    ::: moniker-end

    ::: moniker range="vs-2022"
    :::image type="content" source="media/developer-command-prompt-for-vs/developer-command-prompt-visual-studio-2022.png" alt-text="Screenshot of the Developer Command Prompt for Visual Studio 2022 that shows the clrver tool.":::
    ::: moniker-end

- **Visual Studio Developer PowerShell** - More powerful than a command prompt. For example, you can pass the output of one command (known as a *cmdlet*) to another cmdlet. This shell has the same environment variables set as Developer Command Prompt. Available since Visual Studio 2019.

    ::: moniker range="vs-2022"
    :::image type="content" source="media/developer-command-prompt-for-vs/developer-powershell-visual-studio-2022.png" alt-text="Screenshot of the Developer PowerShell tool in Visual Studio 2022.":::
    ::: moniker-end

Starting in [Visual Studio 2019](https://devblogs.microsoft.com/visualstudio/say-hello-to-the-new-visual-studio-terminal/), Visual Studio includes an integrated **terminal** that can host either of these shells (Developer Command Prompt and Developer PowerShell). You can also open multiple tabs of each shell. The Visual Studio terminal is built on top of [Windows Terminal](/windows/terminal/). To open the terminal in Visual Studio, select **View** > **Terminal**.

::: moniker range="vs-2022"
:::image type="content" source="media/developer-command-prompt-for-vs/visual-studio-2022-terminal-window.png" alt-text="Screenshot of the Visual Studio terminal pane that shows multiple tabs.":::
::: moniker-end

::: moniker range="vs-2019"
:::image type="content" source="media/developer-command-prompt-for-vs/vs-terminal.png" alt-text="Screenshot of the Visual Studio terminal showing multiple tabs.":::
::: moniker-end

> [!TIP]
> This page describes how to use the command-line shells in [Visual Studio](https://visualstudio.microsoft.com/#vs-section). If you're looking for the equivalent in [Visual Studio Code](https://visualstudio.microsoft.com/#vscode-section)&mdash;also known as **VS Code**&mdash;see [Command Line Interface (CLI)](https://code.visualstudio.com/docs/editor/command-line) and [Terminal Basics](https://code.visualstudio.com/docs/terminal/basics).

When you open one of the developer shells from Visual Studio, either as a separate app or in the Terminal window, it opens to the directory of your current solution (if you have a solution loaded). This behavior makes it convenient to run commands against the solution or its projects.

Both shells have specific environment variables set that enable you to use command-line developer tools more easily. After opening one of these shells, you can enter the commands for different utilities without having to know where they're located.

|Popular commands|Description|
|--|--|
|[`MSBuild`](../../msbuild/msbuild-command-line-reference.md)|Build a project or solution|
|[`clrver`](/dotnet/framework/tools/clrver-exe-clr-version-tool)| A [.NET Framework tool](/dotnet/framework/tools/index) for CLR|
|[`ildasm`](/dotnet/framework/tools/ildasm-exe-il-disassembler)|A [.NET Framework tool](/dotnet/framework/tools/index) for disassembler|
|[`dotnet`](/dotnet/core/tools/dotnet)|A [.NET CLI command](/dotnet/core/tools/index)|
|[`dotnet run`](/dotnet/core/tools/dotnet-run)|A [.NET CLI command](/dotnet/core/tools/index)|
|[`CL`](/cpp/build/reference/compiler-command-line-syntax)|C/C++ compile tool|
|[`NMAKE`](/cpp/build/reference/running-nmake)|C/C++ compile tool|
|[`LIB`](/cpp/build/reference/lib-reference)| C/C++ build tool|
|[`DUMPBIN`](/cpp/build/reference/dumpbin-reference)| C/C++ build tool|

## Start in Visual Studio

Follow these steps to open Developer Command Prompt or Developer PowerShell from within Visual Studio:

1. Open Visual Studio.

1. On the menu bar, select **Tools** > **Command Line** > **Developer Command Prompt** or **Developer PowerShell**.

    ::: moniker range="vs-2022"
    :::image type="content" source="media/developer-command-prompt-for-vs/visual-studio-2022-command-line-menu.png" alt-text="Screenshot of the Command Line menu in Visual Studio 2022.":::
    ::: moniker-end

    ::: moniker range="vs-2019"
   ![Screenshot of the Command Line menu in Visual Studio 2019.](./media/developer-command-prompt-for-vs/vs-menu.png)
    ::: moniker-end

## Start from Windows menu

Another way to start the shells is from the Start menu. You may have multiple command prompts, depending on the version of Visual Studio and any additional SDKs and workloads you've installed.

### Windows 11

1. Select **Start** :::image type="content" source="media/developer-command-prompt-for-vs/windows-11-logo-button.png" alt-text="Screenshot of the Start button in Windows 11.":::, and then in the **Type here to search** dialog box, enter either `developer command prompt` or `developer powershell`.

1. Select the App result that's associated with your search text.

### Windows 10

1. Select **Start** ![Screenshot of the Start button in Windows 10.](./media/developer-command-prompt-for-vs/windows-logo-key-graphic.png), and then scroll to the letter **V**.

1. Expand the **Visual Studio 2019** or **Visual Studio 2022** folder.

1. If you're running Visual Studio 2019, select either **Developer Command Prompt for VS 2019** or **Developer PowerShell for VS 2019**. If you're running Visual Studio 2022, select either **Developer Command Prompt for VS 2022** or **Developer PowerShell for VS 2022**.

   Alternatively, you can start typing the name of the shell in the search box on the taskbar, and select the result you want as the result list starts to display the search matches.

   ![An animation that shows the search behavior in Windows 10.](./media/developer-command-prompt-for-vs/windows-10-search.gif)

### Windows 8.1

1. Go to the **Start** screen, by pressing the Windows logo key ![Screenshot of the Windows logo key on the keyboard.](./media/developer-command-prompt-for-vs/windows-logo-key-graphic.png) on your keyboard for example.

1. On the **Start** screen, press **Ctrl**+**Tab** to open the **Apps** list, and then press **V**. This brings up a list that includes all installed Visual Studio command prompts.

1. If you're running Visual Studio 2019, select either **Developer Command Prompt for VS 2019** or **Developer PowerShell for VS 2019**. If you're running Visual Studio 2022, select **Developer Command Prompt for VS 2022** or **Developer PowerShell for VS 2022**.

### Windows 7

1. Select **Start** and then expand **All Programs**.

1. Select **Visual Studio 2019** > **Visual Studio Tools** > **Developer Command Prompt for VS 2019** or **Developer PowerShell for VS 2019**. (If you're running Visual Studio 2022, look for the same items that include "2022" instead of "2019".)

   ![Screenshot of the Windows 7 Start menu with the command prompt highlighted.](./media/developer-command-prompt-for-vs/windows-7-menu.png)

If you have other SDKs installed, such as the [Windows 10 SDK](https://developer.microsoft.com/windows/downloads/windows-10-sdk) or [previous versions](https://developer.microsoft.com/windows/downloads/sdk-archive), you may see additional command prompts. Check the documentation for the individual tools to determine which version of the command prompt you should use.

## Start from file browser

Usually, the shortcuts for the shells you have installed are placed in the **Start Menu** folder for Visual Studio, such as in *%ProgramData%\Microsoft\Windows\Start Menu\Programs\Visual Studio 2019\Visual Studio Tools*. But if searching for the command prompt doesn't produce the expected results, you can try to manually locate the files on your machine.

### Developer Command Prompt

Search for the name of the command prompt file, which is *VsDevCmd.bat*, or go to the Tools folder for Visual Studio, such as *%ProgramFiles%\Microsoft Visual Studio\2022\Community\Common7\Tools* (the path changes according to your Visual Studio version, edition, and installation location).

Once you've located the command prompt file, open it by entering the following command in a regular command prompt window:

::: moniker range="vs-2022"

```cmd
"%ProgramFiles%\Microsoft Visual Studio\2022\Community\Common7\Tools\VsDevCmd.bat"
```

Or enter the following command in the Windows **Run** dialog box:

```cmd
%comspec% /k "C:\Program Files\Microsoft Visual Studio\2022\Community\Common7\Tools\VsDevCmd.bat"
```

::: moniker-end

::: moniker range="vs-2019"

```cmd
"%ProgramFiles(x86)%\Microsoft Visual Studio\2019\Community\Common7\Tools\VsDevCmd.bat"
```

Or enter the following command in the Windows **Run** dialog box:

```cmd
%comspec% /k "C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\Common7\Tools\VsDevCmd.bat"
```

::: moniker-end

> [!TIP]
> Make sure to edit the path to match the version or edition of Visual Studio that you're using.

### Developer PowerShell

Search for a PowerShell script file named *Launch-VsDevShell.ps1*, or go to the Tools folder for Visual Studio, such as *%ProgramFiles(x86)%\Microsoft Visual Studio\2019\Community\Common7\Tools*. (The path changes according to your Visual Studio version, edition, and installation location.) Once you've located the PowerShell file, run it by entering the following command at a Windows PowerShell or PowerShell 6 prompt:

```powershell
& 'C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\Common7\Tools\Launch-VsDevShell.ps1'
```

By default, the Developer PowerShell that launches is configured for the Visual Studio installation whose install path the *Launch-VsDevShell.ps1* file is located in.

> [!TIP]
> The [execution policy](/powershell/module/microsoft.powershell.core/about/about_execution_policies) must be set in order for the cmdlet to run.

The `Launch-VsDevShell.ps1` script works by locating the `Microsoft.VisualStudio.DevShell.dll` PowerShell module in the Visual Studio installation path, loading it, and then invoking the `Enter-VsDevShell` cmdlet. Installed shortcuts, like those in the Start menu, load the module and invoke the cmdlet directly. `Launch-VsDevShell.ps1` is the recommended way to initialize Developer PowerShell interactively or for scripting build automation.

## Command-line arguments

You can use command-line arguments for either of the shells, Developer Command Prompt or Developer PowerShell.

### Target Architecture and Host Architecture

For build tools -- like the C++ compiler -- that create outputs targeting specific CPU architectures, the developer shells can be configured using the appropriate command-line argument. The architecture of the build tool binaries can also be configured by using command-line arguments. This is useful when the build machine is a different architecture than the target architecture.

> [!TIP]
> Beginning with Visual Studio 2022, `msbuild` will default to a 64-bit msbuild.exe binary, regardless of the Host Architecture.

|Shell|Argument|
|--|--|
|Developer Command Prompt|-arch=&lt;Target Architecture&gt;|
|Developer Command Prompt|-host_arch=&lt;Host Architecture&gt;|
|Developer PowerShell|-Arch &lt;Target Architecture&gt;|
|Developer PowerShell|-HostArch &lt;Host Architecture&gt;|

> [!IMPORTANT]
> Developer PowerShell arguments -Arch and -HostArch are only available beginning with [Visual Studio 2022 version 17.1](/visualstudio/releases/2022/release-notes#1710--visual-studio-2022-version-171-newreleasebutton).

The following table lists which architectures are supported, and whether they can be used for Target Architecture or Host Architecture arguments.

|Architecture|Target Architecture|Host Architecture|
|--|--|--|
|x86|Default|Default|
|amd64|Yes|Yes|
|arm|Yes|No|
|arm64|Yes|No|

> [!TIP]
> If you set only Target Architecture, the shells attempt to make the Host Architecture match. This can result in errors when only the Target Architecture is set to a value that's not also supported by Host Architecture.

#### Examples

Start the Developer Command Prompt for Visual Studio 2019 Community Edition on a 64-bit machine, creating build outputs that target 64-bit:
```cmd
"%ProgramFiles(x86)%\Microsoft Visual Studio\2019\Community\Common7\Tools\VsDevCmd.bat" -arch=amd64
```

Start the Developer Command Prompt for Visual Studio 2019 Community Edition on a 64-bit machine, creating build outputs that target arm:
```cmd
"%ProgramFiles(x86)%\Microsoft Visual Studio\2019\Community\Common7\Tools\VsDevCmd.bat" -arch=arm -host_arch=amd64
```

Start the Developer PowerShell for the Community Edition of [Visual Studio 2022 version 17.1](/visualstudio/releases/2022/release-notes#1710--visual-studio-2022-version-171-newreleasebutton) or later on a 64-bit machine, creating build outputs that target arm64:
```powershell
& 'C:\Program Files (x86)\Microsoft Visual Studio\2022\Community\Common7\Tools\Launch-VsDevShell.ps1' -Arch arm64 -HostArch amd64
```

### SkipAutomaticLocation

For Developer PowerShell, the starting directory of the shell is the Visual Studio Project Location. This default locale overrides any other paths, such as working directory. This behavior can be turned off by using the command-line argument `-SkipAutomaticLocation`. This can be useful if you want the shell to stay in the current directory after initialization.

The Project Location can be adjusted in **Tools** > **Options** > **Projects &amp; Solutions** > **Project Location**.

> [!TIP]
> The command-line arguments `-Arch`, `-HostArch`, and `-SkipAutomaticLocation` are supported by both the `Launch-VsDevShell.ps1` script and the `Enter-VsDevShell` cmdlet.

## See also

- [Windows Terminal](/windows/terminal/)
- [.NET Framework Tools](/dotnet/framework/tools/index)
- [Use the Microsoft C++ toolset from the command line](/cpp/build/building-on-the-command-line)
