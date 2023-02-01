---
description: "Gets the size of the object in bytes."
title: IDebugObject::GetSize | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugObject::GetSize
helpviewer_keywords:
- IDebugObject::GetSize method
ms.assetid: 89af423b-36eb-479d-b2de-2693455eca15
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
# IDebugObject::GetSize

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Gets the size of the object in bytes.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetSize(
   out uint pnSize
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetSize( 
   UINT* pnSize
);
```
---

## Parameters
`pnSize`\
[out] Returns the size in bytes.

## Return Value
 If successful, returns S_OK; otherwise, returns an error code.

## Remarks
 Use the [GetValue](../../../extensibility/debugger/reference/idebugobject-getvalue.md) method to retrieve the value as a sequence of bytes.

## See also
- [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md)
- [GetValue](../../../extensibility/debugger/reference/idebugobject-getvalue.md)
