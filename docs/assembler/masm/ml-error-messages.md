---
title: ML 错误消息
ms.date: 08/30/2018
ms.custom: error-reference
f1_keywords:
- vc.errors.ml
helpviewer_keywords:
- MASM (Microsoft Macro Assembler), ML error messages
ms.assetid: e7e164b3-6d65-4b5b-8925-bfbebc043523
ms.openlocfilehash: 2db928d22219d33f89396bb29530680d4b3c8dba
ms.sourcegitcommit: a6d63c07ab9ec251c48bc003ab2933cf01263f19
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "74856938"
---
# <a name="ml-error-messages"></a>ML 错误消息

MASM 组件生成的错误消息分为三个类别：

- **错误。** 这表明出现了阻止实用工具完成其正常过程的严重问题。

- **非致命错误。** 实用工具可能会完成其过程。 如果是这样，则其结果不太可能是所需的结果。

- **列出.** 这些消息指示可能会阻止您获取所需结果的条件。

所有错误消息采用以下形式：

> *实用工具*：*文件名*（*行*）： {*Error_type*} （*代码*）： *Message_text*

其中：

*实用工具*\
发送错误消息的程序。

*文件名*\
包含错误生成条件的文件。

*行*\
错误条件所在的大概行。

*Error_type*\
错误、错误或警告。

*代码*\
唯一的5或6位错误代码。

*Message_text*\
错误条件的简短和一般说明。

## <a name="see-also"></a>另请参阅

[Microsoft 宏汇编程序参考](../../assembler/masm/microsoft-macro-assembler-reference.md)
