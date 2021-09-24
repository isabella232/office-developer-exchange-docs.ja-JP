---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: InternetMessageHeaders 要素には、メールボックス内のアイテムに含まれる一部のインターネット メッセージ ヘッダーのコレクションが含まれています。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERSプロパティを使用します。 EWS およびインターネット メッセージ ヘッダーの詳細については、「EWS、MIME、および不足しているインターネット メッセージ ヘッダーにインターネット メッセージ ヘッダーを取得する」を参照してください。
ms.openlocfilehash: 1ea49f2d5cc31aef09a9bc6d38dff25652696842
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541081"
---
# <a name="internetmessageheaders"></a>InternetMessageHeaders

**InternetMessageHeaders** 要素には、メールボックス内のアイテムに含まれる一部のインターネット メッセージ ヘッダーのコレクションが含まれています。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERSプロパティ **を使用** します。 EWS およびインターネット メッセージ ヘッダーの詳細については [、「EWS、MIME、](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)および不足しているインターネット メッセージ ヘッダー」の「Getting Internet message headers」を参照してください。
  
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
|[InternetMessageHeader](internetmessageheader.md) <br/> |header コレクション内の特定のヘッダーのインターネット メッセージ ヘッダーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼に対する Accept 返信を表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼に対する辞退の返信を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[項目](item.md) <br/> |ストア内のアイテムをExchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮承諾の返信を表します。  <br/> |
   
## <a name="remarks"></a>注釈

次に、EWS マネージ API 拡張プロパティ定義を示します。PR_TRANSPORT_MESSAGE_HEADERS **します。** 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[EWS、MIME、および欠落しているインターネット メッセージ ヘッダー](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

