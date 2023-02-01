---
title: Move Task | Microsoft Docs
description: Learn about the parameters and settings for the MSBuild Move task, which moves files to new locations.
ms.custom: SEO-VS-2020
ms.date: 11/04/2016
ms.topic: reference
dev_langs:
- VB
- CSharp
- C++
helpviewer_keywords:
- MSBuild, Move task
- Move task [MSBuild]
ms.assetid: d1405347-1309-4f18-b565-905408093d59
author: ghogen
ms.author: ghogen
manager: jmartens
ms.technology: msbuild
ms.workload:
- multiple
---
# Move task

Moves files to a new location.

## Parameters

 The following table describes the parameters of the <xref:Microsoft.Build.Tasks.Move> task.

|Parameter|Description|
|---------------|-----------------|
|`DestinationFiles`|Optional <xref:Microsoft.Build.Framework.ITaskItem>`[]` output parameter.<br /><br /> Specifies the list of files to move the source files to. This list is expected to be a one-to-one mapping to the list that is specified in the `SourceFiles` parameter. That is, the first file specified in `SourceFiles` will be moved to the first location specified in `DestinationFiles`, and so forth.|
|`DestinationFolder`|Optional <xref:Microsoft.Build.Framework.ITaskItem> parameter.<br /><br /> Specifies the directory to which you want to move the files.|
|`MovedFiles`|Optional <xref:Microsoft.Build.Framework.ITaskItem>`[]` output parameter.<br /><br /> Contains the items that were successfully moved.|
|`OverwriteReadOnlyFiles`|Optional `Boolean` parameter.<br /><br /> If `true`, overwrites files even if they are marked as read-only files.|
|`SourceFiles`|Required <xref:Microsoft.Build.Framework.ITaskItem>`[]` parameter.<br /><br /> Specifies the files to move.|

## Remarks

 Either the `DestinationFolder` parameter or the `DestinationFiles` parameter must be specified, but not both. If both are specified, the task fails and an error is logged.

 The `Move` task creates folders as required for the desired destination files.

 In addition to having the parameters that are listed in the table, this task inherits parameters from the <xref:Microsoft.Build.Tasks.TaskExtension> class, which itself inherits from the <xref:Microsoft.Build.Utilities.Task> class. For a list of these additional parameters and their descriptions, see [TaskExtension base class](../msbuild/taskextension-base-class.md).

## Examples

The following example moves files from the *source* folder to the *dest* folder. The *source* and *dest* folders are relative to the project file. If *dest* doesn't exist, it is created.

```xml
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <ItemGroup>
    <FilesToMove Include="source\*.*"/>
  </ItemGroup>

  <Target Name="MoveFiles" AfterTargets="Build">
     <Message Text="Moving Files @(FilesToMove)"/>
     <Move SourceFiles="@(FilesToMove)" DestinationFolder="dest">
       <Output 
          TaskParameter="DestinationFiles"
          ItemName="FilesWritten"/>
     </Move>
     <Message Text="@(FilesWritten)"/>
  </Target>
</Project>
```

The following example renames files according to a replacement pattern. It assumes files like *files\original1.txt* and *files\original2.txt* exist and *original.txt* exists at the project level prior to execution. Note the use of the string item function `Replace` to modify the filenames. See [Item functions](item-functions.md).

```xml
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">

  <ItemGroup>
    <FilesToRename Include="files\original*" />    
  </ItemGroup>

  <Target Name="MoveFiles" AfterTargets="Build">
    <Message Text="Rename one file"/>
    <Move SourceFiles="original.txt" DestinationFiles="new.txt"/>
    <Message Text="Renaming files @(FilesToRename)"/>
    <Move SourceFiles="@(FilesToRename)" DestinationFiles="@(FilesToRename->Replace('original', 'new'))" />
  </Target>

</Project>
```

The following examples rename all files in a complete subtree that contain the search text and replacement text in the MSBuild properties. It shows the use of the string property function `Replace` to modify the filename. It also demonstrates the use of the `OverwriteReadOnlyFiles` option.

```xml
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">

  <PropertyGroup>
    <SearchText>original</SearchText>
    <ReplaceText>new</ReplaceText>
  </PropertyGroup>

  <ItemGroup>
    <FilesToRename Include="files\**\*$(SearchText)*" />    
  </ItemGroup>

  <Target Name="MoveFiles" AfterTargets="Build">
    <Message Text="Renaming files @(FilesToRename)"/>
    <Move SourceFiles="@(FilesToRename)"
          OverwriteReadOnlyFiles="true"
          DestinationFiles="@(FilesToRename->Replace($(SearchText), $(ReplaceText)))" />
  </Target>

</Project>
```

You might find it useful to use item metadata to construct the destination file list. Here, the well-known item metadata `%(RelativeDir)` and `%(Filename)` are referenced to construct the modified filenames, in this case to change the extensions for any file in a subtree with the extension `.txt` to `.orig`.

```xml
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">

  <PropertyGroup>
    <NewExtension>orig</NewExtension>
  </PropertyGroup>

  <ItemGroup>
    <FilesToRename Include="files\**\*.txt" />    
  </ItemGroup>

  <Target Name="MoveFiles" AfterTargets="Build">
    <Message Text="Renaming files @(FilesToRename)"/>
    <Move SourceFiles="@(FilesToRename)"
          OverwriteReadOnlyFiles="true"
          DestinationFiles="%(RelativeDir)%(Filename).$(NewExtension)" />
  </Target>

</Project>
```

## See also

- [Tasks](../msbuild/msbuild-tasks.md)
- [Task reference](../msbuild/msbuild-task-reference.md)
