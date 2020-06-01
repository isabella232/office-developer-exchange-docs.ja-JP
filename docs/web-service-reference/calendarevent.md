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
description: CalendarEvent 要素は、固有の予定表アイテムの出現を表します。
ms.openlocfilehash: 8bf37c907ed726e33dd2b1eff9add5d6235704da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459077"
---
# <a name="calendarevent"></a>CalendarEvent

**CalendarEvent**要素は、固有の予定表アイテムの出現を表します。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |予定表イベントの開始を表します。 これは必須の子要素です。  <br/> |
|[EndTime](endtime.md) <br/> |予定表イベントの終了を表します。 これは必須の子要素です。  <br/> |
|[BusyType](busytype.md) <br/> |予定表イベントの空き時間状態セットを表します。 これは必須の子要素です。  <br/> |
|[CalendarEventDetails](calendareventdetails.md) <br/> |予定表イベントに関する追加情報を提供します。 これはオプションの子要素です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarEventArray](calendareventarray.md) <br/> |要求されたユーザーの空き時間情報を表す、一連の一意な予定表アイテムの繰り返しを含みます。  <br/> この要素の XPath 2.0 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a>注釈

予定および会議の時刻は、クライアントのタイムゾーンで返されます。 すべての子要素が発生する順序で一覧表示されます。 この要素によって提供される詳細レベルは、リクエスターに付与されるアクセス許可によって異なります。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

