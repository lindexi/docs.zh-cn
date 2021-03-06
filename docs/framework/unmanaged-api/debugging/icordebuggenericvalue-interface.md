---
description: 了解详细信息： ICorDebugGenericValue 接口
title: ICorDebugGenericValue 接口
ms.date: 03/30/2017
api_name:
- ICorDebugGenericValue
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugGenericValue
helpviewer_keywords:
- ICorDebugGenericValue interface [.NET Framework debugging]
ms.assetid: bc14f408-b359-4c8c-ade2-888ccdf7261b
topic_type:
- apiref
ms.openlocfilehash: 7c81855849d7b72bc509d20072b96bb64f5d395a
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99692025"
---
# <a name="icordebuggenericvalue-interface"></a>ICorDebugGenericValue 接口

"ICorDebugValue" 的子类，适用于所有值。 此接口可为值提供 Get 和 Set 方法。  
  
## <a name="methods"></a>方法  
  
|方法|说明|  
|------------|-----------------|  
|[GetValue 方法](icordebuggenericvalue-getvalue-method.md)|将值复制到指定的缓冲区中。|  
|[SetValue 方法](icordebuggenericvalue-setvalue-method.md)|从指定的缓冲区复制新值。|  
  
## <a name="remarks"></a>备注  

 `ICorDebugGenericValue` 是子接口，因为它是不可远程处理的。  
  
 对于引用类型，该值是引用而不是引用的内容。  
  
 此接口不支持跨计算机或跨进程远程调用。  
  
> [!NOTE]
> 此接口不支持跨计算机或跨进程远程调用。  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头**：CorDebug.idl、CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [调试接口](debugging-interfaces.md)
