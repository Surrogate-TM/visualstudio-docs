---
description: "Retrieves the size of the text at this position in the document."
title: IDebugDocumentText2::GetSize | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugDocumentText2::GetSize
helpviewer_keywords:
- IDebugDocumentText2::GetSize
ms.assetid: bf515a8f-dcee-4004-8f81-543d547ceaae
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
# IDebugDocumentText2::GetSize

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves the size of the text at this position in the document.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetSize( 
   ref uint pcNumLines,
   ref uint pcNumChars
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetSize( 
   ULONG* pcNumLines,
   ULONG* pcNumChars
);
```
---

## Parameters
`pcNumLines`\
[out] Returns the number of lines of text.

`pcNumChars`\
[out] Returns the number of characters of text.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## Remarks

 [C++ only] If a particular value is not desired, pass a NULL for the parameter.

 [C# only] Both parameters must be specified.

## See also
- [IDebugDocumentText2](../../../extensibility/debugger/reference/idebugdocumenttext2.md)
