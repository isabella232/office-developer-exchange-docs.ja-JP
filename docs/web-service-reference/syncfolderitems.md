---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: SyncFolderItems 要素は、ストア フォルダー内のアイテムを同期する要求Exchange定義します。
ms.openlocfilehash: a3e5aa83335a6bc29b832021e227e6adad4092bf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513284"
---
# <a name="syncfolderitems"></a>SyncFolderItems

**SyncFolderItems 要素** は、ストア フォルダー内のアイテムを同期する要求Exchange定義します。 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 **SyncFolderItemsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを識別します。 この要素は必須です。  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダーを表します。 この要素は必須です。  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |要求が成功した後に更新される同期データの base64 エンコード形式が含まれる。 これは、同期状態を識別するために使用されます。 この要素は省略できます。  <br/> |
|[無視](ignore.md) <br/> |同期中にスキップするアイテムを識別します。 この要素は省略できます。  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |同期応答で返される変更の最大数を示します。 この要素は必須です。  <br/> |
|[SyncScope](syncscope.md) <br/> |アイテムまたはアイテムとフォルダーに関連付けられた情報を同期応答で返すかどうかを指定します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

