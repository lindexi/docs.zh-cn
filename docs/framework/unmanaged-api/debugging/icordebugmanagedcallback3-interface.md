---
description: 了解详细信息： ICorDebugManagedCallback3 接口
title: ICorDebugManagedCallback3 接口
ms.date: 03/30/2017
api_name:
- ICorDebugManagedCallback3
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugManagedCallback3
helpviewer_keywords:
- ICorDebugManagedCallback3 interface [.NET Framework debugging]
ms.assetid: a95389d3-cf2e-47a4-9805-61426acc6b65
topic_type:
- apiref
ms.openlocfilehash: 9fb3d44b1d793935ac997e8e4d8d86de4466f7b2
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99801184"
---
# <a name="icordebugmanagedcallback3-interface"></a>ICorDebugManagedCallback3 接口

提供一个回调方法，该方法指示已发出启用的自定义调试器通知。  
  
## <a name="methods"></a>方法  
  
|方法|说明|  
|------------|-----------------|  
|[CustomNotification 方法](icordebugmanagedcallback3-customnotification-method.md)|指示已引发启用的自定义调试器通知。|  
  
## <a name="remarks"></a>备注  

 此接口是 [ICorDebugManagedCallback](icordebugmanagedcallback-interface.md) 和 [ICorDebugManagedCallback2](icordebugmanagedcallback2-interface.md) 接口的逻辑扩展。  
  
> [!NOTE]
> 此接口不支持跨计算机或跨进程远程调用。  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头**：CorDebug.idl、CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [ICorDebugManagedCallback 接口](icordebugmanagedcallback-interface.md)
- [ICorDebugManagedCallback2 接口](icordebugmanagedcallback2-interface.md)
- [调试接口](debugging-interfaces.md)
- [调试](index.md)
