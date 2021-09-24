---
title: Changes (Items)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Changes
api_type:
- schema
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: Changes 要素には、クライアント上のアイテムとサーバー上のアイテムの違いの種類を表す変更の種類のシーケンス配列がExchangeされます。
ms.openlocfilehash: 3c6cbc72e4de10401de12df715129a004f8c5d7e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518793"
---
# <a name="changes-items"></a>Changes (Items)

**Changes 要素** には、クライアント上のアイテムとサーバー上のアイテムの違いの種類を表す変更の種類のシーケンス配列がExchangeされます。 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[Changes (Items)](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
   <ReadFlagChange/>
</Changes>
```

 **SyncFolderItemsChangesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つのアイテムを識別します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つのアイテムを識別します。  <br/> |
|[Delete (ItemSync)](delete-itemsync.md) <br/> |ローカル クライアント ストアで削除する 1 つのアイテムを識別します。  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |アイテムの読 [み取り時に SyncFolderItems](syncfolderitems-operation.md) 操作の応答で返されます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |[SyncFolderItems](syncfolderitems-operation.md)操作要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

