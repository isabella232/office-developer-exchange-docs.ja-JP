---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: CalendarEvent 要素は、一意の予定表アイテムの出現を表します。
ms.openlocfilehash: f7fff7ba511ca12813dd4c2d694e89c97589ba31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759579"
---
# <a name="calendarevent"></a>CalendarEvent

**CalendarEvent**要素は、一意の予定表アイテムの出現を表します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 **CalendarEvent**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[開始時刻](starttime.md) <br/> |予定表イベントの開始を表します。 これは、必須の子要素です。  <br/> |
|[終了時刻](endtime.md) <br/> |予定表のイベントの終了を表します。 これは、必須の子要素です。  <br/> |
|[BusyType](busytype.md) <br/> |予定表イベントの空き時間情報の状態を表します。 これは、必須の子要素です。  <br/> |
|[CalendarEventDetails](calendareventdetails.md) <br/> |カレンダー イベントの追加情報を提供します。 これは、省略可能な子要素です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarEventArray](calendareventarray.md) <br/> |要求されたユーザーの可用性を表す一意の予定表アイテムの出現回数のセットが含まれています。  <br/> この要素への XPath 2.0 の式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>備考

クライアントのタイム ゾーンでは、予定と会議の時刻が返されます。 発生したシーケンスは、すべての子要素の一覧です。 この要素によって提供される詳細のレベルは、要求側に付与するアクセス許可に依存します。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

