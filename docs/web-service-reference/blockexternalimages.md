---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: BlockExternalImages 要素は、HTML テキストの本体で外部の画像がブロックされているかどうかを指定します。
ms.openlocfilehash: 41ab2ec7ec1c24ccbbef037ef1e27431c1fe6811
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759504"
---
# <a name="blockexternalimages"></a>BlockExternalImages

**BlockExternalImages**要素は、HTML テキストの本体で外部の画像がブロックされているかどうかを指定します。 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |GetFolder、FindFolder、または SyncFolderHierarchy の応答に含めるフォルダーのプロパティを識別します。  <br/> |
|[ItemShape](itemshape.md) <br/> |GetItem、FindItem、または SyncFolderItems の応答に含めるコンテンツ アイテムのプロパティを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**True** **BlockExternalImages**要素のテキスト値は、HTML の本文で、外部の画像がブロックされていることを示します。 **False**の値は、外部の画像が許可されていることを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

