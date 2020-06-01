---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: InternetMessageHeaders 要素には、メールボックス内のアイテムに含まれるいくつかのインターネットメッセージヘッダーのコレクションが含まれています。 インターネットメッセージヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネットメッセージヘッダーの詳細については、「EWS、MIME、および不足しているインターネットメッセージヘッダー」の「インターネットメッセージヘッダーの取得」を参照してください。
ms.openlocfilehash: 4719050c02590e021b29173c234466de3fdc58a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467327"
---
# <a name="internetmessageheaders"></a>InternetMessageHeaders

**Internetmessageheaders**要素には、メールボックス内のアイテムに含まれるいくつかのインターネットメッセージヘッダーのコレクションが含まれています。 インターネットメッセージヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。 EWS およびインターネットメッセージヘッダーの詳細については、「 [ews、MIME、および不足しているインターネット](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)メッセージヘッダー」の「インターネットメッセージヘッダーを取得する」を参照してください。
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 **NonEmptyArrayOfInternetHeadersType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[InternetMessageHeader](internetmessageheader.md) <br/> |Headers コレクション内の指定されたヘッダーのインターネットメッセージヘッダーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼への返信を承諾するかを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼への返信を拒否することを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮承諾の返信を表します。  <br/> |
   
## <a name="remarks"></a>注釈

**PR_TRANSPORT_MESSAGE_HEADERS**プロパティの EWS マネージ API 拡張プロパティの定義を次に示します。 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[EWS、MIME、および欠落しているインターネット メッセージ ヘッダー](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

