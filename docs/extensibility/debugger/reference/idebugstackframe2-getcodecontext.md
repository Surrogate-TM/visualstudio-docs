---
description: "Gets the code context for this stack frame."
title: IDebugStackFrame2::GetCodeContext | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugStackFrame2::GetCodeContext
helpviewer_keywords:
- IDebugStackFrame2::GetCodeContext
ms.assetid: 93d66159-a41d-49ef-982f-91bb4d073b74
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
# IDebugStackFrame2::GetCodeContext

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Gets the code context for this stack frame.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetCodeContext ( 
   out IDebugCodeContext2 ppCodeCxt
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetCodeContext ( 
   IDebugCodeContext2** ppCodeCxt
);
```
---

## Parameters
`ppCodeCxt`\
[out] Returns an [IDebugCodeContext2](../../../extensibility/debugger/reference/idebugcodecontext2.md) object that represents the current instruction pointer in this stack frame.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## See also
- [IDebugStackFrame2](../../../extensibility/debugger/reference/idebugstackframe2.md)
- [IDebugCodeContext2](../../../extensibility/debugger/reference/idebugcodecontext2.md)
