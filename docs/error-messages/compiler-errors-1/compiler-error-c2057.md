---
title: 编译器错误 C2057
ms.date: 11/04/2016
f1_keywords:
- C2057
helpviewer_keywords:
- C2057
ms.assetid: 038a99d6-1f5a-42fa-8449-03b4ff11ee0b
ms.openlocfilehash: 37dbc2f6ae0614215f0a3de20baa601b48db9450
ms.sourcegitcommit: 16fa847794b60bf40c67d20f74751a67fccb602e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2019
ms.locfileid: "74742439"
---
# <a name="compiler-error-c2057"></a>编译器错误 C2057

应输入常量表达式

该上下文要求输入常数表达式，即其值在编译时已知的表达式。

编译器在编译时必须知道类型的大小，以便为该类型的实例分配空间。

## <a name="example"></a>示例

下面的示例生成 C2057，并演示如何修复此错误：

```cpp
// C2057.cpp
int i;
int b[i];   // C2057 - value of i is unknown at compile time
int main() {
   const int i = 8;
   int b[i]; // OK - value of i is fixed and known to compiler
}
```

## <a name="example"></a>示例

C 对常数表达式有限制性更强的规则。  下面的示例生成 C2057，并演示如何修复此错误：

```
// C2057b.c
#define ArraySize1 10
int main() {
   const int ArraySize2 = 10;
   int h[ArraySize2];   // C2057 - C does not allow variables here
   int h[ArraySize1];   // OK - uses preprocessor constant
}
```
