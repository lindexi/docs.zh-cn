---
description: 了解详细信息： BC36629：在此上下文中不支持可以为 Null 的类型推理
title: 该上下文中不支持可以为 null 的类型推理
ms.date: 07/20/2015
f1_keywords:
- vbc36629
- bc36629
helpviewer_keywords:
- BC36629
ms.assetid: 0a1e2dbc-d9a4-433d-9306-c5540782b81d
ms.openlocfilehash: 915f964d55068f39b0468e2c47cc6e5538be1a6f
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99795620"
---
# <a name="bc36629-nullable-type-inference-is-not-supported-in-this-context"></a>BC36629：在此上下文中不支持可以为 Null 的类型推理

值类型和结构可以声明为 null。

```vb
Dim a? As Integer
Dim b As Integer?
```

 但是，不能将可为 null 的声明与类型推理结合使用。 下面的示例将导致此错误。

```vb
' Not valid.
' Dim c? = 10
' Dim d? = a
```

 **错误 ID：** BC36629

## <a name="to-correct-this-error"></a>更正此错误

- 使用 `As` 子句将变量声明为可以为 null 的值类型。

## <a name="see-also"></a>请参阅

- [可以为 null 的值类型](../../programming-guide/language-features/data-types/nullable-value-types.md)
- [局部类型推理](../../programming-guide/language-features/variables/local-type-inference.md)
