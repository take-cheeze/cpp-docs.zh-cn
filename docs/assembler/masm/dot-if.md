---
title: .IF
ms.date: 11/05/2019
f1_keywords:
- .IF
helpviewer_keywords:
- .IF directive
ms.assetid: dccc7615-8fc7-4829-9f39-0ee405f6c1e3
ms.openlocfilehash: e8213052dce8d84d62f90d4bc2653435c2b31434
ms.sourcegitcommit: 9ee5df398bfd30a42739632de3e165874cb675c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74398224"
---
# <a name="if-32-bit-masm"></a>.IF （32位 MASM）

生成测试*condition1*的代码（例如，AX > 7），如果该条件为 true，则执行*语句*。 （仅限32位 MASM。）

## <a name="syntax"></a>语法

> **.如果** *condition1*\
> *语句*\
> ⟦ **。ELSEIF** *condition2*\
> *语句*⟧ \
> ⟦ **。ELSE**\
> *语句*⟧ \
> **.ENDIF**

## <a name="remarks"></a>备注

如果为[。否则](../../assembler/masm/dot-else.md)，如果原始条件为 false，则执行其语句。 请注意，将在运行时评估条件。

## <a name="see-also"></a>另请参阅

[指令参考](directives-reference.md)
