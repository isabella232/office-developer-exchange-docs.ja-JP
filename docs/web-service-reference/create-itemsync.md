---
title: Create (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: Create 要素は、ローカル クライアント ストアで作成する 1 つのアイテムを識別します。
ms.openlocfilehash: 2b36fad021c7ccb767eb80b31f71f12ef6cbbd22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510336"
---
# <a name="create-itemsync"></a>Create (ItemSync)

**Create 要素は**、ローカル クライアント ストアで作成する 1 つのアイテムを識別します。 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) 
- [Changes (Items)](changes-items.md) 
- [Create (ItemSync)](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

**SyncFolderItemsCreateOrUpdateType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |作成するアイテムのExchangeを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |作成するExchangeメッセージを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |作成する予定表Exchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |作成する連絡先Exchangeを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |作成する配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |作成する会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |作成する会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |作成する会議の応答を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |作成する会議のキャンセルを表します。  <br/> |
|[タスク](task.md) <br/> |作成するタスクを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |クライアント上のアイテムとクライアント サーバー上のアイテムの違いの種類を表す変更の種類のシーケンス配列をExchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderItems 操作](syncfolderitems-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

