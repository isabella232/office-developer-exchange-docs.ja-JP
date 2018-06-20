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
description: InternetMessageHeaders 要素には、いくつかのメールボックス内の項目に含まれているインターネット メッセージ ヘッダーのコレクションが含まれています。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、PR_TRANSPORT_MESSAGE_HEADERS プロパティを使用します。 EWS およびインターネット メッセージ ヘッダー、seeGetting インターネット メッセージ headersin EWS、MIME、および不足しているインターネット メッセージ ヘッダーに関する詳細については。
ms.openlocfilehash: 2da529a8a3532cebb2791b285b7673c962a2a656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831954"
---
# <a name="internetmessageheaders"></a>InternetMessageHeaders

**InternetMessageHeaders**要素には、いくつかのメールボックス内の項目に含まれているインターネット メッセージ ヘッダーのコレクションが含まれています。 インターネット メッセージ ヘッダーのコレクション全体を取得するには、 **PR_TRANSPORT_MESSAGE_HEADERS**プロパティを使用します。 EWS およびインターネット メッセージ ヘッダーの詳細については、 [EWS、MIME、および不足しているインターネット メッセージ ヘッダー](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)の「取得のインターネット メッセージのヘッダー」を参照してください。
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 **NonEmptyArrayOfInternetHeadersType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[InternetMessageHeader](internetmessageheader.md) <br/> |ヘッダー コレクション内の指定したヘッダーのインターネット メッセージ ヘッダーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼、承諾の返信を表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼を辞退の返信を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に仮承諾の返信を表します。  <br/> |
   
## <a name="remarks"></a>備考

**PR_TRANSPORT_MESSAGE_HEADERS**プロパティのプロパティの定義を拡張する EWS マネージ API は、次のようにします。 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[EWS、MIME、および不足しているインターネット メッセージのヘッダー](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

