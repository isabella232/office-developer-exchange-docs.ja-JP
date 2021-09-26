---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: SavedItemFolderId 要素は、メールボックス内のアイテムを更新、送信、および作成する操作のターゲット フォルダーを識別します。
ms.openlocfilehash: 75245cf842336621aa098c115d62a7802711dd54
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546120"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

**SavedItemFolderId** 要素は、メールボックス内のアイテムを更新、送信、および作成する操作のターゲット フォルダーを識別します。 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |アイテムを更新、送信、および作成する操作のターゲット フォルダーの識別子と変更キーが格納され、Exchangeされます。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |アイテムを更新、送信、および作成する操作の名前付き識別子によってターゲット フォルダーを識別し、Exchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |アイテムストアにアイテムを作成する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |ストア内のアイテムを更新する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |ストア内のアイテムを送信する要求をExchangeします。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

