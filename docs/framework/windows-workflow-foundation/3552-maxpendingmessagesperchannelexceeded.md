---
description: 了解详细信息： 3552-MaxPendingMessagesPerChannelExceeded
title: 3552 - MaxPendingMessagesPerChannelExceeded
ms.date: 03/30/2017
ms.assetid: fc8309d9-eb3a-4636-a6f0-dd0018c1361d
ms.openlocfilehash: 5fb2d27f7d68716cebf2cfaafd21851226a456e6
ms.sourcegitcommit: ddf7edb67715a5b9a45e3dd44536dabc153c1de0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "99631432"
---
# <a name="3552---maxpendingmessagesperchannelexceeded"></a>3552 - MaxPendingMessagesPerChannelExceeded

## <a name="properties"></a>属性  
  
|||  
|-|-|  
|ID|3552|  
|关键字|配额、WFServices|  
|级别|警告|  
|通道|Microsoft-Windows-应用程序服务器-应用程序/分析|  
  
## <a name="description"></a>说明  

 指示达到了中止值“MaxPendingMessagesPerChannel”。  
  
## <a name="message"></a>消息  

 达到了“%1”的中止值“MaxPendingMessagesPerChannel”。 若要增加此限制，请调整 BufferedReceiveServiceBehavior 中的 MaxPendingMessagesPerChannel 属性。  
  
## <a name="details"></a>详细信息  
  
|数据项名称|数据项类型|说明|  
|--------------------|--------------------|-----------------|  
|限制|xs:string|中止值 MaxPendingMessagesPerChannel。|  
|应用程序域|xs:string|由 AppDomain.CurrentDomain.FriendlyName 返回的字符串。|
