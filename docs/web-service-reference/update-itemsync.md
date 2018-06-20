---
title: 更新プログラム (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: 更新プログラム要素は、ローカル クライアント ストアで更新する 1 つの項目を識別します。
ms.openlocfilehash: ef1bd46906152affbe54372472766afc2a6ae8c1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839827"
---
# <a name="update-itemsync"></a>更新プログラム (ItemSync)

**Update**要素は、ローカル クライアント ストアで更新する 1 つの項目を識別します。 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[変更 (アイテム)](changes-items.md)
  
[更新プログラム (ItemSync)](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

 **SyncFolderItemsCreateOrUpdateType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |更新するのには、一般的な Exchange アイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |更新する Exchange 電子メール メッセージを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |更新するのには、Exchange 予定表のアイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange 連絡先を更新する項目を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |更新する配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議を更新するメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |更新する会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |更新するのには会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |更新するのには、会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |更新するタスクを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[変更 (アイテム)](changes-items.md) <br/> |クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems の操作](syncfolderitems-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

