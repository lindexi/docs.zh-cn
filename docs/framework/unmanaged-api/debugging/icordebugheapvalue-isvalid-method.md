---
description: 了解详细信息： ICorDebugHeapValue：： IsValid 方法
title: ICorDebugHeapValue::IsValid 方法
ms.date: 03/30/2017
api_name:
- ICorDebugHeapValue.IsValid
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugHeapValue::IsValid
helpviewer_keywords:
- IsValid method [.NET Framework debugging]
- ICorDebugHeapValue::IsValid method [.NET Framework debugging]
ms.assetid: 68e20e62-203d-46d8-bb91-8d3c61cfacc3
topic_type:
- apiref
ms.openlocfilehash: 27eca844170b31934cd32dad5cf5fccc0b0e324e
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99660773"
---
# <a name="icordebugheapvalueisvalid-method"></a>ICorDebugHeapValue::IsValid 方法

获取一个值，该值指示此 ICorDebugHeapValue 表示的对象是否有效。  
  
 此方法在 .NET Framework 版本2.0 中已弃用。  
  
## <a name="syntax"></a>语法  
  
```cpp  
HRESULT IsValid (  
    [out] BOOL    *pbValid  
);  
```  
  
## <a name="parameters"></a>参数  

 `pbValid`  
 弄一个指向布尔值的指针，该布尔值指示堆上的此值是否有效。  
  
## <a name="remarks"></a>备注  

 如果它已被垃圾回收器回收，则该值无效。  
  
 此方法已被否决。 在 .NET Framework 2.0 中，在调用 [ICorDebugController：： Continue](icordebugcontroller-continue-method.md) 之前，所有值都有效，此时值无效。  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头**：CorDebug.idl、CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]
