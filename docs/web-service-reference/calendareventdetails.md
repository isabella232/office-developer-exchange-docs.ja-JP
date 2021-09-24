---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: CalendarEventDetails 要素は、予定表イベントに関する追加情報を提供します。
ms.openlocfilehash: c332d17b1bb630b9635e64c484b4c5fd989f9845
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516091"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

**CalendarEventDetails 要素は**、予定表イベントに関する追加情報を提供します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
[CalendarEventDetails](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 **CalendarEventDetails**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ID](id.md) <br/> |予定表アイテムのエントリ ID を表します。  <br/> |
|[Subject (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |予定表アイテムの件名を表します。  <br/> |
|[Location (CalendarEventDetails)](location-calendareventdetails.md) <br/> |予定表アイテムの場所フィールドを表します。  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |予定表イベントが会議か予定かを示します。  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |予定表イベントが定期的な予定表アイテムまたは 1 つの予定表アイテムのインスタンスであるかどうかを示します。  <br/> |
|[IsException](isexception.md) <br/> |定期的な予定表アイテムのインスタンスがマスターから変更されるかどうかを示します。  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |予定表イベントにアラームが設定されているかどうかを示します。  <br/> |
|[IsPrivate](isprivate.md) <br/> |予定表アイテムがプライベートかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |一意の予定表アイテムの出現を表します。  <br/> 次に、この要素の XPath 2.0 式を示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>注釈

すべての子要素は、その子要素が発生する順序で一覧表示されます。 
  
[IsPrivate](isprivate.md)要素が **true** の場合 [、CalendarEventDetails](calendareventdetails.md)要素内の他のすべての要素は応答で返されません。 
  
GetUserAvailability 操作は、呼び出し元がターゲット ユーザーの予定表に対する読み取りアクセス権を持たない限り、詳細な発信者情報を返しません。 アクセス許可は、管理シェルを使用Exchange設定できます。
  
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

