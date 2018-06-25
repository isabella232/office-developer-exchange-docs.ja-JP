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
description: WebClientReadFormQueryString 要素は、Outlook Web App 内の項目を参照するのには Outlook Web App エンドポイントへの連結に URL を表します。
ms.openlocfilehash: 8096c14956d132a631b0ade6f2eae12a2bff9c06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840007"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

**WebClientReadFormQueryString**要素は、Outlook Web App 内の項目を参照するのには Outlook Web App エンドポイントへの連結に URL を表します。 
  
```XML
<WebClientReadFormQueryString/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

文字列を表す文字列値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

Outlook Web App の URL のアイテム id は、アイテムの EWS 識別子です。 EWS の項目の識別子が URL エンコードし、アイテムを Outlook Web App の URL を取得するクエリ文字列に追加します。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
### <a name="version-differences"></a>バージョンの相違点

15.0.775.38 (CU3) をビルドするバージョンの Exchange が Exchange Server 2013 でメジャー バージョン 15 で開始および終了を Exchange オンライン バージョン 15.00.0775.009 も返さない正しいクエリ文字列のフラグメント**WebClientReadFormQueryString**要素にします。 
  
15 の主要なバージョンより前のバージョンの Exchange では、Outlook Web App の Url のアイテム id は、Outlook Web App の識別子です。 15 のメジャー バージョンより前の Exchange のバージョンを対象とする場合は、識別子に変換する[ConvertId の操作](convertid-operation.md)を使用する必要です。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

