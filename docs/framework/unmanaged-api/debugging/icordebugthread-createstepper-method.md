---
description: 了解详细信息： ICorDebugThread：： CreateStepper 方法
title: ICorDebugThread::CreateStepper 方法
ms.date: 03/30/2017
api_name:
- ICorDebugThread.CreateStepper
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugThread::CreateStepper
helpviewer_keywords:
- ICorDebugThread::CreateStepper method [.NET Framework debugging]
- CreateStepper method, ICorDebugThread interface [.NET Framework debugging]
ms.assetid: 4657443f-dd12-431b-a648-175c23f13c83
topic_type:
- apiref
ms.openlocfilehash: 378ce28281f4f284c36194f993a53598a9de3854
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99659356"
---
# <a name="icordebugthreadcreatestepper-method"></a>ICorDebugThread::CreateStepper 方法

创建一个 ICorDebugStepper 对象，该对象允许单步执行此 ICorDebugThread 的活动框架。  
  
## <a name="syntax"></a>语法  
  
```cpp  
HRESULT CreateStepper (  
    [out] ICorDebugStepper **ppStepper  
);  
```  
  
## <a name="parameters"></a>参数  

 `ppStepper`  
 弄指向 `ICorDebugStepper` 允许单步执行此线程的活动帧的对象地址的指针。  
  
## <a name="remarks"></a>备注  

 活动框架可能是非托管代码。  
  
 `ICorDebugStepper`接口必须用于执行实际步进。  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头**：CorDebug.idl、CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]
