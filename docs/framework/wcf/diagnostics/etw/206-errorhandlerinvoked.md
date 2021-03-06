---
description: 了解详细信息： 206-ErrorHandlerInvoked
title: 206 - ErrorHandlerInvoked
ms.date: 03/30/2017
ms.assetid: 97340f4d-4e09-4e42-a17a-982b3868dbcf
ms.openlocfilehash: addbcbdea25c7f8e7515b743e98e426476fa0b28
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99783776"
---
# <a name="206---errorhandlerinvoked"></a>206 - ErrorHandlerInvoked

## <a name="properties"></a>属性  
  
|||  
|-|-|  
|ID|206|  
|关键字|疑难解答，ServiceModel|  
|级别|信息|  
|通道|Microsoft-Windows-应用程序服务器-应用程序/分析|  
  
## <a name="description"></a>说明  

 当 `ErrorHandler` 有机会处理在服务操作中发生的异常后，将发出此事件。  
  
## <a name="message"></a>消息  

 调度程序调用了类型为 "%1" 且类型为 "%3" 的 ErrorHandler 的类型为 "%1" 的。 ErrorHandled 为“%2”。  
  
## <a name="details"></a>详细信息  
  
|数据项名称|数据项类型|说明|  
|--------------------|--------------------|-----------------|  
|TypeName|`xs:string`|所调用 `ErrorHandler` 的类型的 CLR FullName。|  
|已处理|`xs:unsignedByte`|如果错误处理程序已处理错误，则为 `true`；否则为 `false`。|  
|ExceptionTypeName|`xs:string`|待处理异常的 CLR FullName。|  
|HostReference|`xs:string`|对于 Web 承载的服务，此字段唯一标识 Web 层次结构中的服务。 其格式定义为 "网站名称应用程序虚拟路径&#124;服务虚拟路径&#124;ServiceName"。 示例： "Default Web Site//Calculatorapplication&#124;/CalculatorService.svc&#124;CalculatorService"。|  
|应用程序域|`xs:string`|由 AppDomain.CurrentDomain.FriendlyName 返回的字符串。|
