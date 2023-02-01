---
title: 'How to: Use the Activity Log | Microsoft Docs'
description: VSPackages can write messages to the activity log. Learn how to use the activity log for debugging VSPackages in retail environments.
ms.custom: SEO-VS-2020
ms.date: 11/04/2016
ms.topic: how-to
helpviewer_keywords:
- VSPackages, debugging
- VSPackages, troubleshooting
ms.assetid: bb3d3322-0e5e-4dd5-b93a-24d5fbcd2ffd
author: leslierichardson95
ms.author: lerich
manager: jmartens
ms.technology: vs-ide-sdk
ms.workload:
- vssdk
---
# How to: Use the activity log

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
VSPackages can write messages to the activity log. This feature is especially useful for debugging VSPackages in retail environments.

> [!TIP]
> The activity log is always turned on. Visual Studio keeps a rolling buffer of the last 100 entries as well as the first 10 entries, which have general configuration information.

## To write an entry to the activity log

1. Insert this code in the <xref:Microsoft.VisualStudio.Shell.Package.Initialize%2A> method or in any other method except the VSPackage constructor:

    ```csharp
    IVsActivityLog log = GetService(typeof(SVsActivityLog)) as IVsActivityLog;
    if (log == null) return;

    int hr = log.LogEntry((UInt32)__ACTIVITYLOG_ENTRYTYPE.ALE_INFORMATION,
        this.ToString(),
        string.Format(CultureInfo.CurrentCulture,
        "Called for: {0}", this.ToString()));
    ```

     This code gets the <xref:Microsoft.VisualStudio.Shell.Interop.SVsActivityLog> service and casts it to an <xref:Microsoft.VisualStudio.Shell.Interop.IVsActivityLog> interface. <xref:Microsoft.VisualStudio.Shell.Interop.IVsActivityLog.LogEntry%2A> writes an informational entry into the activity log using the current cultural context.

2. When the VSPackage is loaded (usually when a command is invoked or a window is opened), the text is written to the activity log.

## To examine the activity log

1. Run Visual Studio with the [/Log](../ide/reference/log-devenv-exe.md) command line switch to write ActivityLog.xml to disk during your session.

2. After closing Visual Studio, find the activity log in the subfolder for Visual Studio data:

   <em>*%AppData%</em>\Microsoft\VisualStudio\\\<version>\ActivityLog.xml*.

3. Open the activity log with any text editor. Here is a typical entry:

   ```
   Called for: Company.MyApp.MyAppPackage ...
   ```
## Troubleshooting Import/Export Issues in Editor Extensions: Access the MEF Composition Error Log
When writing an editor-based extension, you may experience issues if you try to import something that doesn't exist in the current VS install, or if you incorrectly author your import or export.  The primary way to find and address these issues is to reference the **Managed Extensibility Framework (MEF) Composition Error Log**, stored at *%localappdata%\Microsoft\VisualStudio[yourVSVersion]\ComponentModelCache\Microsoft.VisualStudio.Default.err*.  To learn more about using MEF in your extensions, check out [this documentation](../extensibility/managed-extensibility-framework-in-the-editor.md).

## Robust programming

Because the activity log is a service, the activity log is unavailable in the VSPackage constructor.

You should obtain the activity log just before writing to it. Do not cache or save the activity log for future use.

## See also

- [/Log (devenv.exe)](../ide/reference/log-devenv-exe.md)
- <xref:Microsoft.VisualStudio.Shell.Interop.IVsActivityLog>
- <xref:Microsoft.VisualStudio.Shell.Interop.__ACTIVITYLOG_ENTRYTYPE>
- [Troubleshooting VSPackages](../extensibility/troubleshooting-vspackages.md)
- [VSPackages](../extensibility/internals/vspackages.md)
