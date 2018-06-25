---
title: 変更 (アイテム)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: d3139fef-0455-4b89-babd-5d6783b50a58
description: 変更要素には、クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。
ms.openlocfilehash: 8e38597276e3e3051a5c1494619d3220280e401f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759619"
---
# <a name="changes-items"></a>変更 (アイテム)

**変更**要素には、クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[変更 (アイテム)](changes-items.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **SyncFolderItemsChangesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[(ItemSync) を作成します。](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つの項目を識別します。  <br/> |
|[更新プログラム (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つの項目を識別します。  <br/> |
|[(ItemSync) を削除します。](delete-itemsync.md) <br/> |ローカル クライアント ストアで削除するのには 1 つの項目を識別します。  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |アイテムを開封したときに、 [SyncFolderItems 操作](syncfolderitems-operation.md)の応答で返されます。 このプロパティは値の取得のみ可能です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |[SyncFolderItems 操作](syncfolderitems-operation.md)要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems の操作](syncfolderitems-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

