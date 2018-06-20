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
description: SyncFolderItems 要素は、Exchange ストアのフォルダーのアイテムを同期するための要求を定義します。
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839638"
---
# <a name="syncfolderitems"></a>SyncFolderItems

**SyncFolderItems**要素は、Exchange ストアのフォルダーのアイテムを同期するための要求を定義します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。 この要素は必須です。  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期する項目を含むフォルダーを表します。 この要素は必須です。  <br/> |
|[同期状態](syncstate-ex15websvcsotherref.md) <br/> |各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。 これを使用して、同期の状態を識別します。 この要素はオプションです。  <br/> |
|[Ignore](ignore.md) <br/> |同期中にスキップする項目を識別します。 この要素はオプションです。  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |同期応答で返すことができる変更の最大数について説明します。 この要素は必須です。  <br/> |
|[SyncScope](syncscope.md) <br/> |同期応答内のアイテムまたはアイテムおよびフォルダーに関連付けられている情報だけを返すかどうかを指定します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems の操作](syncfolderitems-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

