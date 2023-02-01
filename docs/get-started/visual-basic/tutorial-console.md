---
title: "Tutorial: Create a simple Visual Basic (VB) console app"
description: "In this tutorial, you learn how to create a Visual Basic console application in Visual Studio."
ms.custom: "vs-acquisition, get-started"
ms.date: 02/09/2022
ms.technology: vs-ide-general
ms.prod: visual-studio-windows
ms.topic: tutorial
ms.devlang: vb
author: anandmeg
ms.author: meghaanand
manager: jmartens
dev_langs:
  - vb
ms.workload:
  - "multiple"
# Customer intent: As a novice, I want to create my first app so that I see how Visual Basic works.
---
# Tutorial: Create a simple Visual Basic (VB) console app

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]

This article shows how you'll use Visual Studio to create a simple Visual Basic application, a *console app*. In this app, you ask the user for their name, and then display it back with the current time. You'll also explore some features of the [Visual Studio integrated development environment (IDE)](visual-studio-ide.md), including [source control in Git](/visualstudio/version-control). Visual Basic is a type-safe programming language that's designed to be easy to learn. A console app takes input and displays output in a command-line window, also known as a console.

In this tutorial, you learn how to:

> [!div class="checklist"]
> - Create a Visual Studio project
> - Run the default application
> - Add code to ask for user input
> - Extra credit: Add two numbers
> - Add Git source control
> - Clean up resources

## Prerequisites

If you haven't already installed Visual Studio, go to the [Visual Studio downloads](https://visualstudio.microsoft.com/downloads) page to install it for free.

## Create a project

First, you'll create a Visual Basic app project. The default project template includes all the files you'll need for a runnable app.  

::: moniker range="<=vs-2019"

> [!NOTE]
> Some of the screenshots in this tutorial use the dark theme. If you aren't using the dark theme but would like to, see the [Personalize the Visual Studio IDE and Editor](../../ide/quickstart-personalize-the-ide.md) page to learn how.

::: moniker-end

::: moniker range="vs-2019"

1. Open Visual Studio 2019.

1. In the start window, choose **Create a new project**.

   :::image type="content" source="media/vs-2019/create-new-project-dark-theme.png" alt-text="Screenshot showing the Visual Studio start window with 'Create a new project' selected.":::

1. In the **Create a new project** window, choose **Visual Basic** from the Language list. Next, choose **Windows** from the Platform list and **Console** from the project types list.

   After you apply these language, platform, and project type filters, choose the **Console Application** template, and then choose **Next**.

   :::image type="content" source="media/vs-2019/vb-create-new-project-console-net-core.png" alt-text="Screenshot showing the 'Create a new project' window with 'Visual Basic', 'Windows', and 'Console' selected in the Language, Platform, and Project Type filters and the Console Application project template selected.":::

   > [!NOTE]
   > If you do not see the **Console Application** template, you can install it from the **Create a new project** window. In the **Not finding what you're looking for?** message, choose the **Install more tools and features** link.
   >
   > :::image type="content" source="media/vs-2019/not-finding-what-looking-for.png" alt-text="Screenshot showing the 'Install more tools and features' link from the 'Not finding what you're looking for' message in the 'Create new project' window.":::
   >
   > Then, in the Visual Studio Installer, choose the **.NET Core cross-platform development** workload.
   >
   > :::image type="content" source="media/vs-2019/dot-net-core-xplat-dev-workload.png" alt-text="Screenshot showing the .NET Core cross-platform development workload in the Visual Studio Installer.":::
   >
   > After that, choose the **Modify** button in the Visual Studio Installer. You might be prompted to save your work. Next, choose **Continue** to install the workload. Then, return to step 2 in this [Create a project](#create-a-project) procedure.

1. In the **Configure your new project** window, enter *WhatIsYourName* in the **Project name** box. Then, choose **Next**.

   :::image type="content" source="media/vs-2019/vb-name-your-project-whatname.png" alt-text="Screenshot showing the 'Configure your new project' window with the Project name field set to'WhatIsYourName'.":::

1. In the **Additional information** window, **.NET 5.0 (Current)** should already be selected for your target framework. If not, select **.NET 5.0 (Current)**. Then, choose **Create**.

   :::image type="content" source="media/vs-2019/vb-target-framework.png" alt-text="Screenshot showing the 'Additional information' window with '.NET 5.0 (Current)' selected in the Target Framework field.":::

   Visual Studio opens your new project.

::: moniker-end

::: moniker range=">=vs-2022"

1. Open Visual Studio.

1. On the start window, choose **Create a new project**.

   :::image type="content" source="media/vs-2022/create-new-project-dark-theme.png" alt-text="Screenshot showing the Visual Studio start window with 'Create a new project' selected.":::

1. In the **Create a new project** window, choose **Visual Basic** from the Language list. Next, choose **Windows** from the Platform list and **Console** from the Project types list.

   After you apply these language, platform, and project type filters, choose the **Console App** template, and then choose **Next**.

   :::image type="content" source="media/vs-2022/vb-create-new-project-console-net-core.png" alt-text="Screenshot showing the 'Create a new project' window with 'Visual Basic', 'Windows', and 'Console' selected in the Language, Platform, and Project Type filters and the Console App project template selected.":::

   > [!NOTE]
   > If you do not see the **Console App** template, you can install it from the **Create a new project** window. In the **Not finding what you're looking for?** message, choose the **Install more tools and features** link.
   >
   > :::image type="content" source="media/vs-2022/not-finding-what-looking-for.png" alt-text="Screenshot showing the 'Install more tools and features' link from the 'Not finding what you're looking for' message in the 'Create new project' window.":::
   >
   > Then, in the Visual Studio Installer, choose the **.NET desktop development** workload.
   >
   > :::image type="content" source="media/vs-2022/dot-net-core-xplat-dev-workload.png" alt-text="Screenshot showing the .NET desktop development workload in the Visual Studio Installer.":::
   >
   > After that, choose the **Modify** button in the Visual Studio Installer. You might be prompted to save your work. Next, choose **Continue** to install the workload. Then, return to step 2 in this [Create a project](#create-a-project) procedure.

1. In the **Configure your new project** window, enter *WhatIsYourName* in the **Project name** box. Then, choose **Next**.

   :::image type="content" source="media/vs-2022/vb-name-your-project-whatname.png" alt-text="Screenshot showing the 'Configure your new project' window with the Project name field set to'WhatIsYourName'.":::

1. In the **Additional information** window, **.NET 6.0 (Long-term support)** should already be selected for your target framework. If not, select **.NET 6.0 (Long-term support)**. Then, choose **Create**.

   :::image type="content" source="media/vs-2022/vb-target-framework.png" alt-text="Screenshot showing the 'Additional information' window with '.NET 6.0 (Long-term support)' selected in the Framework field.":::

   Visual Studio opens your new project.

::: moniker-end

## Run the app

After you select your Visual Basic project template and name your project, Visual Studio creates a *Program.vb* file. The default code calls the <xref:System.Console.WriteLine%2A> method to display the literal string "Hello World!" in the console window.

There are two ways to run this code, inside Visual Studio in *debug mode*, and from your computer as a regular *standalone* app.

### Run the app in debug mode

::: moniker range="vs-2019"

   :::image type="content" source="media/vs-2019/vb-ide-default-code.png" alt-text="Screenshot showing the default 'Hello World!' code.":::

1. Select the **WhatIsYourName** button or press **F5** to run the default code in Debug mode.

   :::image type="content" source="media/vs-2019/vb-ide-whatisyourname-button.png" alt-text="Screenshot showing the 'What Is Your Name' button highlighted in the Visual Studio toolbar.":::

1. When the app runs in the Microsoft Visual Studio Debug Console, "Hello World!" displays. Press any key to close the debug console window and end the app:

    :::image type="content" source="media/vs-2019/vb-console-hello-world-press-any-key.png" alt-text="Screenshot showing 'Hello World!' and the 'Press any key to close this window' messages.":::

::: moniker-end

::: moniker range=">=vs-2022"

   :::image type="content" source="media/vs-2022/vb-ide-default-code.png" alt-text="Screenshot showing the default 'Hello World!' code.":::

1. Select the **WhatIsYourName** button or press **F5** to run the default code in Debug mode.

   :::image type="content" source="media/vs-2022/vb-ide-whatisyourname-button.png" alt-text="Screenshot showing the 'What Is Your Name' button highlighted in the Visual Studio toolbar.":::

1. When the app runs in the Microsoft Visual Studio Debug Console, "Hello World!" displays. Press any key to close the debug console window and end the app:

    :::image type="content" source="media/vs-2022/vb-console-hello-world-press-any-key.png" alt-text="Screenshot showing 'Hello World!' and the 'Press any key to close this window' messages.":::

::: moniker-end

### Run the app as a standalone

To see the output outside of Visual Studio, in a system console window, build and run the executable (.exe file). 

::: moniker range="vs-2019"

1. In the **Build** menu, choose **Build Solution**.

1. In **Solution Explorer**, right-click on **WhatIsYourName** and choose **Open File in File Explorer**.

1. In **File Explorer**, navigate to the **bin\Debug\net5.0** directory and run **WhatIsYourName.exe**.

1. The `Main` procedure terminates after its single statement executes and the console window closes immediately. To keep the console visible until the user presses a key, see the next section.

::: moniker-end

::: moniker range="vs-2022"

1. In the **Build** menu, choose **Build Solution**.

1. In **Solution Explorer**, right-click on **WhatIsYourName** and choose **Open File in File Explorer**.

1. In **File Explorer**, navigate to the **bin\Debug\core6.0** directory and run **WhatIsYourName.exe**.

1. The `Main` procedure terminates after its single statement executes and the console window closes immediately. To keep the console visible until the user presses a key, see the next section.

::: moniker-end

## Add code to ask for user input

Next, you'll add Visual Basic code that prompts you for your name and then displays it along with the current date and time. In addition, you'll add code that pauses the console window until the user presses a key.

::: moniker range="vs-2019"

1. Enter the following Visual Basic code after the `Sub Main(args As String())` line and before the `End Sub` line, replacing the <xref:System.Console.WriteLine%2A> line:

     ```vb
     Console.Write("Please enter your name: ")
     Dim name = Console.ReadLine()
     Dim currentDate = DateTime.Now
     Console.WriteLine($"Hello, {name}, on {currentDate:d} at {currentDate:t}")
     Console.Write("Press any key to continue...")
     Console.ReadKey(True)
     ```

   - <xref:System.Console.Write%2A> and <xref:System.Console.WriteLine%2A> write a string to the console. 
   - <xref:System.Console.ReadLine%2A> reads input from the console, in this case a string. 
   - <xref:System.DateTime> represents a datetime, and <xref:System.DateTime.Now> returns the current time. 
   - <xref:System.Console.ReadKey> pauses the app and waits for a keypress.

   :::image type="content" source="media/vs-2019/vb-code-window-whatisyourname-dark.png" alt-text="Screenshot showing the code for the 'Program.vb' file in the 'WhatIsYourName' project loaded in the Visual Basic code editor.":::

1. Select the **WhatIsYourName** button or press **F5** to build and run your first app in Debug mode.

1. When the debug console window opens, enter your name. Your console window should look similar to the following screenshot:

   :::image type="content" source="media/vs-2019/vb-console-enter-your-name.png" alt-text="Screenshot showing the debug console window with 'Please enter your name', the date and time, and 'Press any key to continue' messages.":::

1. Press any key to end the app, and then press any key to close the debug console window.

::: moniker-end

::: moniker range=">=vs-2022"

1. Enter the following Visual Basic code after the `Sub Main(args As String())` line and before the `End Sub` line, replacing the <xref:System.Console.WriteLine%2A> line:

     ```vb
     Console.Write("Please enter your name: ")
     Dim name = Console.ReadLine()
     Dim currentDate = DateTime.Now
     Console.WriteLine($"Hello, {name}, on {currentDate:d} at {currentDate:t}")
     Console.Write("Press any key to continue...")
     Console.ReadKey(True)
     ```

   - <xref:System.Console.Write%2A> and <xref:System.Console.WriteLine%2A> write a string to the console. 
   - <xref:System.Console.ReadLine%2A> reads input from the console, in this case a string. 
   - <xref:System.DateTime> represents a datetime, and <xref:System.DateTime.Now> returns the current time. 
   - <xref:System.Console.ReadKey> pauses the app and waits for a keypress.

   :::image type="content" source="media/vs-2022/vb-code-window-whatisyourname-dark.png" alt-text="Screenshot showing the code for the 'Program.vb' file in the 'WhatIsYourName' project loaded in the Visual Basic code editor.":::

1. Select the **WhatIsYourName** button or press **F5** to build and run your first app in Debug mode.

1. When the debug console window opens, enter your name. Your console window should look similar to the following screenshot:

   :::image type="content" source="media/vs-2022/vb-console-enter-your-name.png" alt-text="Screenshot showing the debug console window with 'Please enter your name', the date and time, and 'Press any key to continue' messages.":::

1. Press any key to end the app, and then press any key to close the debug console window.

::: moniker-end

Now that your new code is in the app, build and run the executable (.exe file) in a system console window, as described previously in [Run the app as a standalone](#run-the-app-as-a-standalone). Now when you press a key, the app exits, which closes the console window.

## Extra credit: Add two numbers

This example shows how to read in numbers, rather than a string, and do some arithmetic. Try changing your code from:

```vb
Module Program
    Sub Main(args As String())
        Console.Write("Please enter your name: ")
        Dim name = Console.ReadLine()
        Dim currentDate = DateTime.Now
        Console.WriteLine($"Hello, {name}, on {currentDate:d} at {currentDate:t}")
        Console.Write("Press any key to continue...")
        Console.ReadKey(True)
    End Sub
End Module
```

to:

```vb
Module Program
    Public num1 As Integer
    Public num2 As Integer
    Public answer As Integer
    Sub Main(args As String())
        Console.Write("Type a number and press Enter")
        num1 = Console.ReadLine()
        Console.Write("Type another number to add to it and press Enter")
        num2 = Console.ReadLine()
        answer = num1 + num2
        Console.WriteLine("The answer is " & answer)
        Console.Write("Press any key to continue...")
        Console.ReadKey(True)
    End Sub
End Module
```

And then run the updated app as described under "[Run the app](#run-the-app)".

[!INCLUDE[../includes/git-source-control.md](../includes/git-source-control.md)]

## Clean up resources

If you're not going to continue to use this app, delete the project.

1. In **Solution Explorer**, right-click on **WhatIsYourName** to open the context menu for your project. Then, select **Open Folder in File Explorer**.

1. Close Visual Studio.

1. In the **File Explorer** dialog, go up two levels of folders.

1. Right-click on the **WhatIsYourName** folder and select **Delete**.

## Next steps

Congratulations on completing this tutorial! To learn more, see the following tutorial.

> [!div class="nextstepaction"]
> [Build a library with Visual Basic and the .NET Core SDK in Visual Studio](/dotnet/core/tutorials/vb-library-with-visual-studio)

## See also

* [Visual Basic language walkthroughs](/dotnet/visual-basic/walkthroughs)
* [Visual Basic language reference](/dotnet/visual-basic/language-reference/index)
* [IntelliSense for Visual Basic code files](../../ide/visual-basic-specific-intellisense.md)
