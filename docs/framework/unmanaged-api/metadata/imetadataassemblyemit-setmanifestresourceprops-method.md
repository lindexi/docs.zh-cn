---
description: 了解详细信息： IMetaDataAssemblyEmit：： SetManifestResourceProps 方法
title: IMetaDataAssemblyEmit::SetManifestResourceProps 方法
ms.date: 03/30/2017
api_name:
- IMetaDataAssemblyEmit.SetManifestResourceProps
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- IMetaDataAssemblyEmit::SetManifestResourceProps
helpviewer_keywords:
- SetManifestResourceProps method [.NET Framework metadata]
- IMetaDataAssemblyEmit::SetManifestResourceProps method [.NET Framework metadata]
ms.assetid: ef77efd1-849c-4e51-ba92-7ee3d2bf0339
topic_type:
- apiref
ms.openlocfilehash: 0d5022c4acc562f9e77cec4ba080815db410862b
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99721016"
---
# <a name="imetadataassemblyemitsetmanifestresourceprops-method"></a>IMetaDataAssemblyEmit::SetManifestResourceProps 方法

修改指定的 `ManifestResource` 元数据结构。  
  
## <a name="syntax"></a>语法  
  
```cpp  
HRESULT SetManifestResourceProps (  
    [in] mdManifestResource  mr,  
    [in] mdToken             tkImplementation,
    [in] DWORD               dwOffset,  
    [in] DWORD               dwResourceFlags  
);  
```  
  
## <a name="parameters"></a>参数  

 `mr`  
 中 `ManifestResource` 用于指定要修改的元数据结构的标记。  
  
 `tkImplementation`  
 中 `File` `AssemblyRef` 映射到资源提供程序的标记，类型为或。  
  
 `dwOffset`  
 中文件中资源的起始位置的偏移量。  
  
 `dwResourceFlags`  
 中指定资源特性的标志值的按位组合。  
  
## <a name="remarks"></a>备注  

 若要创建 `ManifestResource` 元数据结构，请使用 [IMetaDataAssemblyEmit：:D efinemanifestresource](imetadataassemblyemit-definemanifestresource-method.md) 方法。  
  
## <a name="requirements"></a>要求  

 **平台：** 请参阅 [系统要求](../../get-started/system-requirements.md)。  
  
 **标头：** Cor  
  
 **库：** 用作 MsCorEE.dll 中的资源  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [IMetaDataAssemblyEmit 接口](imetadataassemblyemit-interface.md)
