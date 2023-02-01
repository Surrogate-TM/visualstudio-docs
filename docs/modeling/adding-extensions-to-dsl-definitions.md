---
title: Add extensions to domain-specific language definitions
description: Learn how the DSL Definition extension allows you to create a package of extensions to a domain-specific language (DSL).
ms.custom:
- SEO-VS-2020
- kr2b-contr-experiment
ms.date: 06/22/2022
ms.topic: conceptual
author: mgoertz-msft
ms.author: mgoertz
manager: jmartens
ms.technology: vs-ide-modeling
ms.workload:
  - "multiple"
---

# Add extensions to DSL definitions

[!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]

DSL Definition extension allows you to create a package of extensions for a domain-specific language (DSL). The DSL extension, which is contained in a Visual Studio Integration Extension (VSIX), can be installed on a user's computer in the same manner as a DSL. The other features can be dynamically enabled and disabled at runtime. DSLs don't have to be explicitly designed for the extension. Extensions can be designed later, or by third parties, without altering the extended DSL.

## DSL extension features

DSL extensions can include the following features:

- Properties for model and presentation elements
- Decorators for shapes and connectors
- Classes, relationships, shapes, and connectors
- Validation constraints
- Toolbox items and tabs

A user of an extended DSL can create and save a model that contains instances of the added features. The model can be read by other users who have installed the appropriate extension. Users who haven't installed the extension can't use the extra features. They can update and save a model without losing the extra features.

[!INCLUDE[modeling_sdk_info](includes/modeling_sdk_info.md)]

## Next steps

- [Related blog posts](https://devblogs.microsoft.com/devops/the-visual-studio-modeling-sdk-is-now-available-with-visual-studio-2017/)
