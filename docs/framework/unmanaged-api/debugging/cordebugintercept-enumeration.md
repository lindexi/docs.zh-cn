---
description: 了解详细信息： CorDebugIntercept 枚举
title: CorDebugIntercept 枚举
ms.date: 03/30/2017
api_name:
- CorDebugIntercept
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- CorDebugIntercept
helpviewer_keywords:
- CorDebugIntercept enumeration [.NET Framework debugging]
ms.assetid: 3d5b642e-7ef2-428b-a5ae-509c35ed461a
topic_type:
- apiref
ms.openlocfilehash: ddd17aff309396fdcda37c731ff907224ee17db2
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99661969"
---
# <a name="cordebugintercept-enumeration"></a>CorDebugIntercept 枚举

指示可截获（即可单步执行）的代码的类型。  
  
## <a name="syntax"></a>语法  
  
```cpp  
typedef enum CorDebugIntercept {  
    INTERCEPT_NONE                = 0x0,  
    INTERCEPT_CLASS_INIT          = 0x01,  
    INTERCEPT_EXCEPTION_FILTER    = 0x02,  
    INTERCEPT_SECURITY            = 0x04,  
    INTERCEPT_CONTEXT_POLICY      = 0x08,  
    INTERCEPT_INTERCEPTION        = 0x10,  
    INTERCEPT_ALL                 = 0xffff  
} CorDebugIntercept;  
```  
  
## <a name="members"></a>成员  
  
|成员|说明|  
|------------|-----------------|  
|`INTERCEPT_NONE`|未截获任何代码。|  
|`INTERCEPT_CLASS_INIT`|可以截获构造函数。|  
|`INTERCEPT_EXCEPTION_FILTER`|可以截获异常筛选器。|  
|`INTERCEPT_SECURITY`|可以截获强制保护的代码。|  
|`INTERCEPT_CONTEXT_POLICY`|可以截获上下文策略。|  
|`INTERCEPT_INTERCEPTION`|未使用。|  
|`INTERCEPT_ALL`|可以截获所有代码。|  
  
## <a name="remarks"></a>备注  

 使用 [ICorDebugStepper：： SetInterceptMask](icordebugstepper-setinterceptmask-method.md) 方法来建立可以截获的代码类型。  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头**：CorDebug.idl、CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [调试枚举](debugging-enumerations.md)
