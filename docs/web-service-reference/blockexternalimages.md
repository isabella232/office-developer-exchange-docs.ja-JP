---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: BlockExternalImages 要素は、HTML テキスト本文で外部イメージをブロックするかどうかを指定します。
ms.openlocfilehash: 82ddb7e53f351324783fa39e3b76c9c0534b8193
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543584"
---
# <a name="blockexternalimages"></a>BlockExternalImages

**BlockExternalImages** 要素は、HTML テキスト本文で外部イメージをブロックするかどうかを指定します。 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |GetFolder、FindFolder、または SyncFolderHierarchy 応答に含めるフォルダー プロパティを識別します。  <br/> |
|[ItemShape](itemshape.md) <br/> |GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**BlockExternalImages** 要素のテキスト値 **が true** の場合、外部イメージは HTML 本文でブロックされます。 false の値 **は** 、外部イメージが許可されている場合を示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

