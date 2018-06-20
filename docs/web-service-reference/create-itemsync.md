---
title: (ItemSync) を作成します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: 作成要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。
ms.openlocfilehash: 39056bcaab3577b1b729421118a45571910922fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759795"
---
# <a name="create-itemsync"></a>(ItemSync) を作成します。

**作成**要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[変更 (アイテム)](changes-items.md)
  
[(ItemSync) を作成します。](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

 **SyncFolderItemsCreateOrUpdateType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |作成する一般的な Exchange アイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |作成する Exchange 電子メール メッセージを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |作成するのには、Exchange 予定表のアイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange 連絡先を作成する項目を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |作成する配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議を作成するメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |作成する会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |作成する会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |作成する会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |作成するタスクを表します。  <br/> |
   
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

