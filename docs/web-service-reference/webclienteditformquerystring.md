---
title: WebClientEditFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WebClientEditFormQueryString
api_type:
- schema
ms.assetid: 9e571021-d58f-424b-8db2-48cf683533dc
description: WebClientEditFormQueryString 要素は、outlook web app エンドポイントに連結して Outlook Web App 内のアイテムを編集するための URL を表します。
ms.openlocfilehash: d6f20d1342746a764f754a6b20633a7bded3f6c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464988"
---
# <a name="webclienteditformquerystring"></a>WebClientEditFormQueryString

**Webclienteditformquerystring**要素は、outlook web app エンドポイントに連結して Outlook web app 内のアイテムを編集するための URL を表します。 
  
```XML
<WebClientEditFormQueryString/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、文字列を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

Exchange Online など、Exchange Server 2013 以降のバージョンの Exchange では、 [Webclientreadformquerystring](webclientreadformquerystring.md)要素の情報を使用して、Outlook Web App の下書きアイテムを開き、その UI を使用して下書きアイテムを編集します。 **Webclienteditformquerystring**要素は、exchange Online を含む exchange Server 2013 以降の exchange のバージョンには適用されません。 
  
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

