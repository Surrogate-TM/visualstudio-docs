---
description: "This method gets the size of a field, in bytes."
title: IDebugField::GetSize | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugField::GetSize
helpviewer_keywords:
- IDebugField::GetSize method
ms.assetid: 73329924-3751-4f44-af54-5986b7943374
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
# IDebugField::GetSize

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
This method gets the size of a field, in bytes.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetSize(
   out uint pdwSize
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetSize( 
   DWORD* pdwSize
);
```
---

## Parameters
`pdwSize`\
[out] Returns the size.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## Remarks
 All fields have a type and all types have a size. For example, a field with a type of byte has a size of 1 byte.

## See also
- [IDebugField](../../../extensibility/debugger/reference/idebugfield.md)
