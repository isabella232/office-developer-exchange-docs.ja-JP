---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: SyncFolderItems 要素は、Exchange ストアフォルダー内のアイテムを同期する要求を定義します。
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465150"
---
# <a name="syncfolderitems"></a>SyncFolderItems

**Syncfolderitems**要素は、Exchange ストアフォルダー内のアイテムを同期する要求を定義します。 
  
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
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダを表します。 この要素は必須です。  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |要求が成功するたびに更新される同期データの base64 でエンコードされた形式が含まれます。 これは、同期状態を識別するために使用されます。 この要素は省略できます。  <br/> |
|[無視](ignore.md) <br/> |同期中にスキップするアイテムを識別します。 この要素は省略できます。  <br/> |
|[Maxの戻り値](maxchangesreturned.md) <br/> |同期応答で返すことができる変更の最大数を示します。 この要素は必須です。  <br/> |
|[SyncScope](syncscope.md) <br/> |同期応答でアイテムまたはアイテムとフォルダーの関連情報のみを返すかどうかを指定します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

