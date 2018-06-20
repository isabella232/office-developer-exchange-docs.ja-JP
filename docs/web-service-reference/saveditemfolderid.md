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
description: SavedItemFolderId 要素は、更新、送信、およびメールボックス内のアイテムを作成する操作のターゲット フォルダーを識別します。
ms.openlocfilehash: c57a7fb4abc2f7ee7b599f56f016811d6ff2c21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833277"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

**SavedItemFolderId**要素は、更新、送信、およびメールボックス内のアイテムを作成する操作のターゲット フォルダーを識別します。 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |更新、送信、および Exchange ストア内の項目を作成する操作の対象となるフォルダーの識別子と変更キーが含まれています。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |更新、送信、および Exchange ストア内の項目を作成する操作の名前付きの識別子では、対象となるフォルダーを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Exchange ストア内のアイテムを作成する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Exchange ストア内の項目を更新する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Exchange ストア内のアイテムを送信する要求を定義します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   

