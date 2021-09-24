---
title: Delete (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- schema
ms.assetid: 4f372d57-2e39-46af-9d83-6c8c55108587
description: Delete 要素は、ローカル クライアント ストアで削除する 1 つのアイテムを識別します。
ms.openlocfilehash: ae8a34506791a2b0e09aea4c7af40ffbba34d523
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519864"
---
# <a name="delete-itemsync"></a>Delete (ItemSync)

**Delete 要素は**、ローカル クライアント ストアで削除する 1 つのアイテムを識別します。 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)  
- [Changes (Items)](changes-items.md)  
- [Delete (ItemSync)](delete-itemsync.md)
  
```xml
<Delete>
   <ItemId/>
</Delete>
```

**SyncFolderItemsDeleteType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。  <br/> |
   
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

