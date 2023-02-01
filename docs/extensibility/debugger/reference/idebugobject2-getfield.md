---
description: "Gets the type of this object."
title: IDebugObject2::GetField | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugObject2::GetField
helpviewer_keywords:
- IDebugObject2::GetField method
ms.assetid: add6a6b5-e752-47dd-9613-29206ea809b0
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
# IDebugObject2::GetField

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Gets the type of this object.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetField(
   out IDebugField ppField
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetField(
 IDebugField** ppField
);
```
---

## Parameters
`ppField`\
[out] Returns an [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) object if not a null value.

## Return Value
 If successful, returns S_OK; otherwise, returns an error code.

## Remarks
 A field describes the type of the object.

## See also
- [IDebugObject2](../../../extensibility/debugger/reference/idebugobject2.md)
- [IDebugField](../../../extensibility/debugger/reference/idebugfield.md)
