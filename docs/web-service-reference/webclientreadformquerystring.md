---
title: WebClientReadFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WebClientReadFormQueryString
api_type:
- schema
ms.assetid: 13e8871a-32a6-4bb9-9493-864c4c07efff
description: WebClientReadFormQueryString 要素は、outlook web app エンドポイントに連結して Outlook Web App 内のアイテムを読み取るための URL を表します。
ms.openlocfilehash: d7102ef288c0aafa6cdada09eda321b546edddb7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464981"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

**Webclientreadformquerystring**要素は、outlook web app エンドポイントに連結して Outlook web app 内のアイテムを読み取るための URL を表します。 
  
```XML
<WebClientReadFormQueryString/>
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
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、文字列を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

Outlook Web App URL のアイテム識別子は、アイテムの EWS 識別子です。 EWS のアイテム識別子を URL でエンコードし、クエリ文字列に追加して、アイテムの Outlook Web App の URL を取得することができます。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
### <a name="version-differences"></a>バージョンの相違点

メジャーバージョン15以降のバージョンの Exchange と Exchange Server 2013 のビルド 15.0.775.38 (CU3) および Exchange Online バージョン15.00.0775.009 は、 **Webclientreadformquerystring**要素に正しいクエリ文字列フラグメントを返しません。 
  
メジャーバージョン15より前のバージョンの Exchange では、Outlook Web App Url のアイテム識別子は Outlook Web App 識別子です。 メジャーバージョン15より前のバージョンの Exchange を対象としている場合は、変換[tid 操作](convertid-operation.md)を使用して識別子を変換する必要があります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

