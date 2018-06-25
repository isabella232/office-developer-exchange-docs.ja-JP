---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: FoldersToIgnore 要素は、会話でアイテムを取得するときに無視されるフォルダーの一覧を識別します。 無視されたフォルダー内のすべての会話項目は GetConversationItems の応答に返されません。
ms.openlocfilehash: 96c094996c601e685dc1c7e6b869a790ce7d74a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760580"
---
# <a name="folderstoignore"></a>FoldersToIgnore

**FoldersToIgnore**要素は、会話でアイテムを取得するときに無視されるフォルダーの一覧を識別します。 無視されたフォルダー内のすべての会話項目は**GetConversationItems**の応答に返されません。 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[フォルダー Id](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)
  
### <a name="parent-elements"></a>親要素

[GetConversationItems](getconversationitems.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

