---
description: "Retrieves the base indices (lower bounds) for each index given the number of dimensions in the array."
title: IDebugArrayObject2::GetBaseIndices | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
helpviewer_keywords:
- GetBaseIndices
- IDebugArrayObject2::GetBaseIndices
ms.assetid: 882951a2-3da0-49bf-8d1e-7daedd13ffe6
author: leslierichardson95
ms.author: lerich
manager: jmartens
ms.technology: vs-ide-debug
ms.workload:
- vssdk
dev_langs:
- CPP
- CSharp
---
# IDebugArrayObject2::GetBaseIndices

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves the base indices (lower bounds) for each index given the number of dimensions in the array.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetBaseIndices (
   uint       dwRank,
   out uint[] dwIndices
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetBaseIndices (
   DWORD  dwRank,
   DWORD* dwIndices
);
```
---

## Parameters
`dwRank`\
[in] The number of dimensions (rank) of the array.

`dwIndices`\
[out] The base indices (lower bounds) for the array.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## Remarks
 As an example, this function would return '5' for the array created by the following C# code:

```
int[] lengths = { 12 };
int[] lowerbounds = { 5 };
Array.CreateInstance(typeof(int), lengths, lowerbounds);
```

## See also
- [IDebugArrayObject2](../../../extensibility/debugger/reference/idebugarrayobject2.md)
