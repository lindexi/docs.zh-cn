---
description: '了解详细信息：整数数据类型 (Visual Basic) '
title: Integer 数据类型
ms.date: 01/31/2018
f1_keywords:
- vb.Integer
- Integer
helpviewer_keywords:
- numbers [Visual Basic], whole
- enumerated values [Visual Basic]
- whole numbers
- integral data types [Visual Basic]
- integer numbers
- numbers [Visual Basic], integer
- integers [Visual Basic], data types
- literal type characters [Visual Basic], I
- integers [Visual Basic], types
- data types [Visual Basic], integral
- '% identifier type character'
- data types [Visual Basic], assigning
- identifier type characters [Visual Basic], %
- I literal type character [Visual Basic]
- Integer data type
ms.assetid: a8f233b4-4be3-455c-861b-05af2fbb6c60
ms.openlocfilehash: 8c60bf19ecd44ca7c9972cbfeb4ee2197bcb137c
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99792201"
---
# <a name="integer-data-type-visual-basic"></a>整数数据类型 (Visual Basic) 

保存 32 位（4 字节）带符号整数，值的范围为 -2,147,483,648 到 2,147,483,647。  
  
## <a name="remarks"></a>备注

 `Integer` 数据类型为 32 位处理器提供了优化性能。 其他整数类型在内存中的加载和存储的速度都要稍慢一些。  
  
 `Integer` 的默认值为 0。  

## <a name="literal-assignments"></a>文本赋值

可以声明和初始化 `Integer` 变量，方法是向其分配十进制文本、十六进制文本、八进制文本，或者从 Visual Basic 2017) 二进制文本开始 (。 如果整数文本在 `Integer` 范围之外（即，如果它小于 <xref:System.Int32.MinValue?displayProperty=nameWithType> 或大于 <xref:System.Int32.MaxValue?displayProperty=nameWithType>），会发生编译错误。

在以下示例中，表示为十进制、十六进制和二进制文本且等于 90,946 的整数被分配给 `Integer` 值。

[!code-vb[integer](../../../../samples/snippets/visualbasic/language-reference/data-types/numeric-literals.vb#Int)]  

> [!NOTE]
> 使用前缀 `&h` 或 `&H` 表示十六进制文本，使用前缀 `&b` 或表示 `&B` 二进制文本，使用前缀 `&o` 或 `&O` 表示八进制文本。 十进制文本没有前缀。

从 Visual Basic 2017 开始，还可以使用下划线字符 `_` 作为数字分隔符来增强可读性，如下面的示例所示。

[!code-vb[integer](../../../../samples/snippets/visualbasic/language-reference/data-types/numeric-literals.vb#IntS)]  

从 Visual Basic 15.5 开始，还可以使用下划线字符 (`_`) 作为前缀和十六进制、二进制或八进制数字之间的前导分隔符。 例如：

```vb
Dim number As Integer = &H_C305_F860
```

[!INCLUDE [supporting-underscores](../../../../includes/vb-separator-langversion.md)]

数字文本还可包含 `I` 用于表示数据类型的 [类型字符](../../programming-guide/language-features/data-types/type-characters.md) `Integer` ，如下面的示例所示。

```vb
Dim number = &H_035826I
```

## <a name="programming-tips"></a>编程提示

- **互操作注意事项。** 如果与不是为 .NET Framework 编写的组件（如自动化或 COM 对象）交互，请记住， `Integer` 在其他环境中具有不同的数据宽度 (16 位) 。 如果将一个 16 位自变量传递给此类组件，请在新的 Visual Basic 代码中将其声明为 `Short` 而不是 `Integer`。  
  
- **扩大.** `Integer` 数据类型加宽到 `Long`、`Decimal`、`Single` 或 `Double`。 这意味着，你可以将 `Integer` 转换为这些类型中的任意类型，而不会遇到 <xref:System.OverflowException?displayProperty=nameWithType> 错误。  
  
- **键入字符。** 将文本类型字符 `I` 追加到文本会将其强制转换为 `Integer` 数据类型。 将标识符类型字符 `%` 追加到任何标识符会将其强制转换为 `Integer`。  
  
- **Framework 类型。** .NET Framework 中的对应类型是 <xref:System.Int32?displayProperty=nameWithType> 结构。  
  
## <a name="range"></a>范围

如果尝试将整型变量设置为其类型范围以外的数字，则将出错。 如果尝试将其设置为小数，则数字将向上或向下舍入为最接近的整数值。 如果数字同样接近两个整数值，则值将舍入为最接近的偶数整数。 这种做法可将因单方向持续舍入中点值而导致的舍入误差降到最低。 下面的代码演示了舍入的示例。  

```vb  
' The valid range of an Integer variable is -2147483648 through +2147483647.  
Dim k As Integer  
' The following statement causes an error because the value is too large.  
k = 2147483648  
' The following statement sets k to 6.  
k = 5.9  
' The following statement sets k to 4  
k = 4.5  
' The following statement sets k to 6  
' Note, Visual Basic uses banker’s rounding (toward nearest even number)  
k = 5.5  
```

## <a name="see-also"></a>请参阅

- <xref:System.Int32?displayProperty=nameWithType>
- [数据类型](index.md)
- [Long 数据类型](long-data-type.md)
- [Short 数据类型](short-data-type.md)
- [Type Conversion Functions](../functions/type-conversion-functions.md)
- [转换摘要](../keywords/conversion-summary.md)
- [有效使用数据类型](../../programming-guide/language-features/data-types/efficient-use-of-data-types.md)
