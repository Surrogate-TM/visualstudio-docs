---
description: "Gets the language information for this code context."
title: IDebugCodeContext2::GetLanguageInfo | Microsoft Docs
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugCodeContext2::GetLanguageInfo
helpviewer_keywords:
- IDebugCodeContext2::GetLanguageInfo
ms.assetid: 03002ef1-9fe6-44b6-b23b-ef7b86b2b21b
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
# IDebugCodeContext2::GetLanguageInfo

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Gets the language information for this code context.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetLanguageInfo( 
   ref string pbstrLanguage,
   ref Guid pguidLanguage
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetLanguageInfo( 
   BSTR* pbstrLanguage,
   GUID* pguidLanguage
);
```
---

## Parameters
`pbstrLanguage`\
[in, out] Returns a string that contains the name of the language, such as "C++."

`pguidLanguage`\
[in, out] Returns the GUID for the language of the code context, for example, `guidCPPLang`.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## Remarks
 At least one of the parameters must return a non-null value.

## See also
- [IDebugCodeContext2](../../../extensibility/debugger/reference/idebugcodecontext2.md)
