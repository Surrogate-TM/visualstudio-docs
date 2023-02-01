---
description: "Sets the value of the object from a consecutive series of bytes."
title: IDebugObject::SetValue | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugObject::SetValue
helpviewer_keywords:
- IDebugObject::SetValue method
ms.assetid: d652e09c-cdc1-4519-8116-d7c743f5679b
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
# IDebugObject::SetValue

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Sets the value of the object from a consecutive series of bytes.

## Syntax

### [C#](#tab/csharp)
```csharp
int SetValue(
   byte[] pValue,
   uint   nSize
);
```
### [C++](#tab/cpp)
```cpp
HRESULT SetValue( 
   BYTE* pValue,
   UINT  nSize
);
```
---

## Parameters
`pValue`\
[in] An array of bytes representing the new value.

`nSize`\
[in] The size of the value in bytes.

## Return Value
 If successful, returns S_OK; otherwise, returns an error code.

## Remarks
 The values in the array are copied into this [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md) object, replacing any existing value. The size of the new value can be larger or smaller than the existing value. This `IDebugObject` cannot be a null reference.

## See also
- [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md)
- [GetValue](../../../extensibility/debugger/reference/idebugobject-getvalue.md)
