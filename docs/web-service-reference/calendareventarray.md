---
title: CalendarEventArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEventArray
api_type:
- schema
ms.assetid: a00f7f56-d7f1-429d-ae02-97043718c864
description: CalendarEventArray 要素には、要求されたユーザーの可用性を表す一意の予定表アイテムの出現のセットが含まれる。
ms.openlocfilehash: 6faf9d85139ce99a6a60da5a05f171a229843b92
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526835"
---
# <a name="calendareventarray"></a>CalendarEventArray

**CalendarEventArray 要素には**、要求されたユーザーの可用性を表す一意の予定表アイテムの出現のセットが含まれる。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 **ArrayOfCalendarEvent**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |一意の予定表アイテムの出現を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |特定のユーザーの可用性情報が含まれる。  <br/> 次に、この要素の XPath 2.0 式を示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a>注釈

この要素によって提供される詳細レベルは、要求者に付与されるアクセス許可によって異なります。 この要素は [、FreeBusyViewType 要素が FreeBusy、FreeBusyMerged、Detailed、](freebusyviewtype.md)または **DetailedMerged に設定されている場合に含まれます**。   要求されたタイム ウィンドウに予定表アイテムが存在しない場合、この要素には子要素は含めされません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

