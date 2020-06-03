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
description: Changes 要素には、クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列が含まれています。
ms.openlocfilehash: 6fda7b5602f172bae84ad7b211db2811def4f883
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463266"
---
# <a name="changes-items"></a>変更 (アイテム)

**Changes**要素には、クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカルクライアントストアに作成する単一のアイテムを識別します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカルクライアントストアで更新する単一のアイテムを識別します。  <br/> |
|[削除 (ItemSync)](delete-itemsync.md) <br/> |ローカルクライアントストアで削除する単一のアイテムを識別します。  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |アイテムが読み取られたときに、 [Syncfolderitems 操作](syncfolderitems-operation.md)の応答で返されます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |[Syncfolderitems 操作](syncfolderitems-operation.md)要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
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

