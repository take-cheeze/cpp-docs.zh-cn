---
title: .SAFESEH
ms.date: 11/05/2019
f1_keywords:
- .SAFESEH
helpviewer_keywords:
- registering functions as exception handlers
- SAFESEH directive
- .SAFESEH directive
ms.assetid: 6eaac8c4-c46f-47ae-8a66-f5cfeb267e43
ms.openlocfilehash: df9798800da293e5e0b4f545a8442380b7ff9408
ms.sourcegitcommit: 9ee5df398bfd30a42739632de3e165874cb675c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/22/2019
ms.locfileid: "74397987"
---
# <a name="safeseh-32-bit-masm"></a>.SAFESEH （32位 MASM）

将函数注册为结构化异常处理程序。 （仅限32位 MASM。）

## <a name="syntax"></a>语法

> **.SAFESEH** *标识符*

## <a name="remarks"></a>备注

*标识符*必须为本地定义的[进程](../../assembler/masm/proc.md)或[EXTRN](../../assembler/masm/extrn.md)过程的 ID。 不允许使用[标签](../../assembler/masm/label-masm.md)。 此.SAFESEH 指令需要[/safeseh](../../assembler/masm/ml-and-ml64-command-line-reference.md)命令行选项。

有关结构化异常处理程序的详细信息，请参阅[/SAFESEH](../../build/reference/safeseh-image-has-safe-exception-handlers.md)。

例如，若要注册安全的异常处理程序，请创建新的 MASM 文件（如下所示），使用/safeseh 进行组合，然后将其添加到链接的对象。

```asm
.386
.model  flat
MyHandler   proto
.safeseh    MyHandler
end
```

## <a name="see-also"></a>另请参阅

[指令参考](directives-reference.md)
