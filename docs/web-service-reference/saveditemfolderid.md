---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: SavedItemFolderId 要素は、メールボックス内のアイテムの更新、送信、および作成を行う操作のターゲットフォルダーを指定します。
ms.openlocfilehash: 8e18b8863a54aa4e9d6e65f7a54e20904f5a9599
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465276"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

**SavedItemFolderId**要素は、メールボックス内のアイテムの更新、送信、および作成を行う操作のターゲットフォルダーを指定します。 
  
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
|[FolderId](folderid.md) <br/> |Exchange ストア内のアイテムの更新、送信、および作成を行う操作のターゲットフォルダーの識別子および変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Exchange ストア内のアイテムを更新、送信、および作成する操作について、ターゲットフォルダーを名前付き識別子で識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Exchange ストア内のアイテムを作成するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Exchange ストア内のアイテムを更新する要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Exchange ストア内のアイテムを送信するための要求を定義します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

