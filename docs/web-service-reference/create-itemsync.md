---
title: Create (ItemSync)
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
ms.openlocfilehash: d49e54c64f7bd53dcb296d998a856c20570d81be
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353946"
---
# <a name="create-itemsync"></a>Create (ItemSync)

**作成**要素は、ローカル クライアント ストアに作成する 1 つの項目を識別します。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |作成する一般的な Exchange アイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |作成する Exchange 電子メール メッセージを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |作成するのには、Exchange 予定表のアイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange 連絡先を作成する項目を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |作成する配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議を作成するメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |作成する会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |作成する会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |作成する会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |作成するタスクを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderItems 操作](syncfolderitems-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

