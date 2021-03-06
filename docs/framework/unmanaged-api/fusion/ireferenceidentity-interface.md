---
description: 了解详细信息： IReferenceIdentity 接口
title: IReferenceIdentity 接口
ms.date: 03/30/2017
api_name:
- IReferenceIdentity
api_location:
- fusion.dll
api_type:
- COM
f1_keywords:
- IReferenceIdentity
helpviewer_keywords:
- IReferenceIdentity interface [.NET Framework fusion]
ms.assetid: 9180ac5a-7019-4716-9f83-8a91d157239a
topic_type:
- apiref
ms.openlocfilehash: a29aaa1f4fb928c136af4168619d27900537c779
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99800040"
---
# <a name="ireferenceidentity-interface"></a>IReferenceIdentity 接口

表示对代码对象的唯一签名的引用。  
  
## <a name="methods"></a>方法  
  
|方法|说明|  
|------------|-----------------|  
|`IReferenceIdentity::Clone`|获取一个指向与 `IReferenceIdentity` 此相同的新实例的接口指针 `IReferenceIdentity` ，指定的特性更改除外。|  
|`IReferenceIdentity::EnumAttributes`|获取一个接口指针，该指针指向 `IEnumIDENTITY_ATTRIBUTE` 包含与此关联的特性的实例 `IReferenceIdentity` 。|  
|`IReferenceIdentity::GetAttribute`|获取指定命名空间中具有指定名称的特性的值。|  
|`IReferenceIdentity::SetAttribute`|将具有指定命名空间和指定名称的特性设置为指定值。|  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头：** 隔离。h  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [合成接口](fusion-interfaces.md)
- [IEnumIDENTITY_ATTRIBUTE 接口](ienumidentity-attribute-interface.md)
