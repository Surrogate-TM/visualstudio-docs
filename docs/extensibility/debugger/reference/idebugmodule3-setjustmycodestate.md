---
description: "Marks the module as being user code or not."
title: IDebugModule3::SetJustMyCodeState | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugModule3::SetJustMyCodeState
helpviewer_keywords:
- IDebugModule3::SetJustMyCodeState
ms.assetid: 68f8166d-ef64-49ae-ad5e-79604f43bbd4
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
# IDebugModule3::SetJustMyCodeState

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Marks the module as being user code or not.

## Syntax

### [C#](#tab/csharp)
```csharp
int SetJustMyCodeState(
   int fIsUserCode
);
```
### [C++](#tab/cpp)
```cpp
HRESULT SetJustMyCodeState(
   BOOL fIsUserCode
);
```
---

## Parameters
`fIsUserCode`\
[in] Nonzero (`TRUE`) if the module should be considered user code, zero (`FALSE`) if it should not.

## Return Value
 If successful, returns `S_OK`; otherwise, returns error code.

## See also
- [IDebugModule3](../../../extensibility/debugger/reference/idebugmodule3.md)
